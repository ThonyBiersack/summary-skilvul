# SUMMARY WEEK 2
## JS Scope

1. scope ada dua tipe yaitu ada block scope dan fucntion scope
  - block scope digunakan oleh bahasa c dan java sedangkan javascript menggunakan funtion scope
  - perbedaan block scope dengan function scope apa?, perbedaan nya saya akan tunjukan dengan code dibawah
  ``` int i = 2
      if ( i % 2 = 0){
        bool genap = true;
      }
      if(genap){
        ptintg ("genap!")
      }```
  kode diatas akan menghasilkan undefined atau error karena variabel genap hanya bisa diakses pada scope pertama.. ohh iya code diatas merupakan 
  contoh code dalam bahasa c
  
  ``` let i = 2
      if(i % 2 == 0){
        var genap = true
      }
      if(genap){
        console.log("genap!")
      }```
  nah dalam javascript kode diatas tidak akan undefined karena javascript sifatnya function scope
2. karena saya sedang belajar javascript jadi saya akan bahas function scope. menurut saya ada yang unik dalam fucntion scope ini, apa yang membuat unik langsung saja 
kita ke contoh nya 
  ``` var a = 1
      fucntion coba(){
        a = 2
      }
      coba();
      console.log(a) ```
  kode diatas akan menampikan nilai 2 kenapa karena didalam function tidak memakai tipe data jadi variable a didalam function akan ditimpakan ke luar function lalu 
  variable a tersebut menjadi global. lalu apa yang terjadi jika variable a di luar di hapus?, maka jawaban nya akan tetap sama yaitu akan menghasil kan 2 karena 
  jika tempat untuk menampung variable a di dalam function maka javascript akan otomatis membuat varibale nya sendiri di lilngkup global.
3. ada juga cara untuk mengatasi agar variable didalam scope tidak di oper menjadi global scope yaitu dengan cara mengetikan "use strict" di global scope maka javascript tidak akan mengoper variable a yang tidak ada tipe data nya ke lingkup global.
