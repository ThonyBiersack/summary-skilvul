# SUMMARY WEEK 2

## JS Scope DAN FUNCITON

1. scope ada dua tipe yaitu ada block scope dan fucntion scope
  - block scope digunakan oleh bahasa c dan java sedangkan javascript menggunakan funtion scope
  - perbedaan block scope dengan function scope apa?, perbedaan nya saya akan tunjukan dengan code dibawah

  ```markdown
  int i = 2
      if ( i % 2 = 0){
        bool genap = true;
      }
      if(genap){
        ptintg ("genap!")
      }
  ```


  kode diatas akan menghasilkan undefined atau error karena variabel genap hanya bisa diakses pada scope pertama.. ohh iya code diatas merupakan 
  contoh code dalam bahasa c
  
  ```
   let i = 2
      if(i % 2 == 0){
        var genap = true
      }
      if(genap){
        console.log("genap!")
      }

  ```

  nah dalam javascript kode diatas tidak akan undefined karena javascript sifatnya function scope


2. karena saya sedang belajar javascript jadi saya akan bahas function scope. menurut saya ada yang unik dalam fucntion scope ini, apa yang membuat unik langsung saja 
kita ke contoh nya 

```
  var a = 1
      fucntion coba(){
        a = 2
      }
      coba();
      console.log(a)

```

  kode diatas akan menampikan nilai 2 kenapa karena didalam function tidak memakai tipe data jadi variable a didalam function akan ditimpakan ke luar function lalu 
  variable a tersebut menjadi global. lalu apa yang terjadi jika variable a di luar di hapus?, maka jawaban nya akan tetap sama yaitu akan menghasil kan 2 karena 
  jika tempat untuk menampung variable a di dalam function maka javascript akan otomatis membuat varibale nya sendiri di lilngkup global.

3. ada juga cara untuk mengatasi agar variable didalam scope tidak di oper menjadi global scope yaitu dengan cara mengetikan "_use strict_" di global scope maka javascript tidak akan mengoper variable a yang tidak ada tipe data nya ke lingkup global.

## DATA TYPE BUILT IN METHOD

1. lanjott ke materi data type built in method, maksudnya apa tuh?. jadi javascript itu menyediakan syntax tambahan atau bantuan untuk bisa mengetahui tipe data ini tuh apa string atau integer atau boolean contoh nya 

``` 
  let hewan = "kucing"
  console.log(typeof hewan) 
```

console.log diatas akan menampilkan tipe data yang ada di variable hewan yaitu _string_
2. ada juga method untuk mencari string didalam sebuah kata kucing misalkan `console.log(hewan.includes("g"))` nah method tersebut akan menampilkan hasil boolean apakah benar disebuah kalimat kucing ada huruf g?, jika benar akan menampilkan _true_ jika salah akan menampilkan _false_

3. selain itu ada cara untuk merubah kalimat menjadi kapital semua dengan menggunakan method `.toUpperCase` dan untuk merubah menajdi huruf kecil semua bisa menggunakan `.toLowecase`

4. selanjutnya ada method untuk menampilkan suatu karakter, misalkan kita mau tau karater apa yang ada di huruf pertama pada kalimat kucing, nah kita bisa menggunakan method `.charAt(angka)`

5. berikutnya ada method `.includes('karakter')` method tersebut berguna untuk memastikan apakah benar ada huruf ini di dalam kalimat tersebut.

6. kemudian ada javascript math, apa saja yang bisa dilakukan oleh javscrpt math sbb:
  - `Math.PI`, untuk menghitung diameter lingkaran
  - `Math.sqrt`, untuk menghitung akar kuadrat
  - `Math.abs`, untuk merubah nilai negative menjadi positive
  - `Math.pow`, untuk menghitung pangkat
  - `Math.round`, untuk menentukan angka bulat jika nilai nya ada koma
  - `Math.floor`, untuk membulatkan nilai ke bawah
  - `Math.ceil`, untuk membulatkan nilai ke atas

## DATA TYPE PRIMITIVE DAN NON PRIMITIVE

1. data type yang primitive adalah data yang tidak mempunyai object dan tidak memiliki method dan property. ada 7 data type yang primitive yaitu :
  - string
  - number
  - big int
  - boolean
  - undefined
  - symbol
  - null
2. data type yang non primitive itu type data yang bisa menampung nilai. contoh nya sebagai berikut
  - object dan array

## DOM

1. apa itu dom, dom itu untuk mengambil id atau juga bisa memanipulasi file html, selain itu juga dom bisa mengubah tampilan css pada html. 
contoh:
```
  <!doctype html>
  <html>
  <head>
  </head>
  <body>
    <h1>hallo</h1>
  </body>
  <html>
```
misalkan kita ingin mengambil tag h1 menggunakan javascript dengan cara
```
  document.getElementsByTagName('h1')[0].innerText
```
2. selanjutnya ada cara untuk mengambil data dari h1 dan dijadikan data untuk paragraf, sbb
  - pertama buat dulu tag `<p>`tapi tidak usah di isi apa apa
  - lalu simpan data yang berada di tag h1 kedalam varible javascript
  ```
    const h1= document.getElementsByaTagName('h1')[0].innerText
  ```
  - setelah itu panggil tag p menggunakan javascript lalu kembalikan value yang ada di variable const h1
  ```
    document.getElementsBytagName('p')[0].innertText = h1
  ```
  - setelah itu nanti akan muncul di tag p html
3. setelah itu ada cara untuk mendapatkan value dari tag input agar ditampilkan dalam pargraf atau heading sbb

  - buat tag input di html
  - buat juga tag button dan berikan onclick didalam nya yang berisikan dari nama function yang akan dibuat
  - buat function di javascript untuk menampung method nya 
  ```
      <!doctype html>
  <html>
  <head>
  </head>
  <body>
    <h1>hallo</h1>
    <input />
    <button onclick= test>click me!</button>
    <p></p>
  </body>
  <html>
  ```
  diatas adalah kondisi di file html

  ```
    function test(){
      const masukan= document.getElementsByTagName('input')[0].value
      document.getElementsByTagName('p')[0].innerText = masukan
    }
  ```
  diatas adalah kondisi di file javascript
  - diatas adalah cara menampilkan data inputan menggunakan javascript
