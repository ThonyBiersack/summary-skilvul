# summary-week 1

## Unix Command Line Interface (CLI)

1. apa itu shell, shell adalah sebuah terminal untuk berinteraksi dengan system operasi
    - contoh nya seperti di windows ada namanya powershell, itu salah satu terminal untuk berkomunikasi dengan system operasi micrososft
2. apa itu CLI, Command Line Interface, sebuah terminal untuk mengerjakan tugas tertentu dengan menggunakan perintah berbentuk teks, sebenarnya powershell dan CLI itu sama saja yang membedakan itu kalau CLI dasar nya, kalau Shell itu pendalaman nya. jadi perintah perintah CLI bisa digunakan di power shell, kita bisa mengibaratkan powershell itu sebagai dewanya CLI.
    - contoh CLI di microsoft yaitu seperti CMD selain CMD juga ada git, fungsi dari kedua aplikasi tersebut yaitu untuk mengerjakan tugas tertentu dan tentu nya tugas tersebut bukan tugas yang bisa dikerjakan oleh powershell. 
3. selanjutnya Struktur Sistem File. Struktur sistem file di windows bentuk nya tree, biasanya di windows itu ada drive c yang biasa nya untuk menyinpan system lalu yang disebut tree itu sub sub folder dari drive c lalu sub folder tersebut juga bisa ditambah sub folder nah itu lah yang dinamakan tree atau bahasa simple saya folder nya bisa bercabang cabang.
4. lalu kita masuk ke command/perintah di CLI yang pertama ada command '*pwd*' perintah ini untuk melihat posisi kita berada di file mana atau di directory mana.
5. selanjutnya untuk mengetahui isi dari sebuah direktori bisa menggunakan command '*ls*' ketika kita menggunakan command tersebut kita akan mengetahui file apa saja yang ada di dalam direktori tersebut atau folder tersebut
6. setelah itu ada command untuk berpindah dari folder a ke b 
    - contoh: di laptop saya punya 2 driver C dan D, ketika membuka terminal posisi saya otomatis pasti ada di drive c dan saya ingin berpindah ke drive d caranya tinggal menggunakan command "*cd D:(backslash)*" kemudian akan langsung berpindah ke drive D
7. berikutnya ada command yang bisa melihat isi file yaitu command '*cat*' selain command itu juga ada '*head*' dan '*tail*' command tersebut berguna untuk melihat isi file yang ada pada direktori, cara penggunaan nya yaitu dengan mengetikan "*cat (nama file)*".
8. lanjut ke command berikutnya itu berfungsi untuk membuat directory atau membuat folder yaitu dengan command '*mkdir*', cara penggunaannya seperti berikut '*mkdir (nama folder)*', lalu ada juga command untuk membuat file yaitu command '*touch*' penggunaan command tersebut itu tinggal ketik "*touch (namafile)*'
9. ngomong ngomong soal membuat folder & file ada juga command untuk menghapus file & folder, untuk menghapus folder kita bisa menggunakan command '*rm -r (nama folder/directory)*' lalu kalo mau hapus file hilangkan -r nya jadi command nya seperti ini '*rm (nama file)*'
10. selain menhapus bisa juga memindahkan atau mengcopy dan merename file & folder dengan command '*mv dan cp*', kita command mv terlebih dahulu, 
    - command mv berfungsi untuk memindahkan file/folder selain itu juga command tersebut bisa juga digunakan untuk merename file/folder. cara penggunaan command mv untuk memindahkan file yaitu dengan mengetikan '*mv (file yang mau dipindahkan) (tujuan direktori)*', untuk memindahkan folder/directory sama saja bedanya ada tambahan -r setelah command jadi command nya seperti ini '*mv -r (nama folder/direktori) (tujuan direktori)*'.
    - command cp berfungsi untuk mengkloning atau mengcopy file/folder, untuk mengcopy file menggunakan command '*cp (nama file) (tujuan paste)*' lalu untuk folder sama seperti di command mv ditambahkan -r setelah command nya jadi seperti ini '*cp -r (nama folder) (tujuan paste)*'
## git & github

1. kenapa kita harus memakai git dan github? karena bagi programmer git dan github itu penting, kenapa bisa penting karena git bisa memberikan data apa saja yang berubah dan siapa yang ngerubahnya, selain itu juga dengan ada nya github para developer bisa mengerjakan bareng atau biasa collab.
2. apa bedanya git dan github, bedanya yaitu git adalah perangkat lunak berbentuk command line yang mengelola riwayat kode sumber kalo github itu sistem layanan hosting untuk repository git.
3. cara kerja git dan github, pertama kita mempunya sebuah projek direktori di komputer kita lalu kita tambahkan ke staging area, setelah masuk ke staging area file itu di commit + tambahkan komentar atau message apa yang telah di tambahkan atau di perbarui, abis itu file tersebut akan di simpan di git repository.
4. cara membuat repository sbb:
        - buat direktori/folder untuk menyimpan file project
        - setelah itu klik kanan pada folder tersebut lalu klik *git bash here* dan nanti muncul terminal
        - lalu ketikan *git init* agar folder tersebut menjadi repository
        - pergi ke github kita buat juga repository disitu caranya gampang tinggal klak klik karena bersifat gui
        - balik lagi ke folder project, kita buat file project disitu misalkan index.html yang berisi test. 
        - berikutnya kita ketikan di git dengan command *git add .*
        - selanjutnya commit *commit -m "nambahin file index.html*
        - lalu remote ke github command nya *git remote add origin + link*
        - abis itu di push ke github *git push -u origin master*
5. cara mengclone repository github ke folder komputer, command nya sebagai berikut *git clone git@github.com:NamaPemilik/NamaRepository.git* jika sudah tekan enter.

## HTML & CSS
1. apa peran html pada website, perannya yaitu untuk membuat kerangka dari tampilan website lalu di warnai atau di hias oleh css
2. selanjutnya ada beberapa tools pendukung untuk menggunakan html yaitu bisa menggunakan text editor, browser, serta plugin pendukung seperti live server
3. saya juga sudah membuat web sederhana, kebetulan juga itu tugas dari skilvul bagian kelas skilpath berikut ini saya kasih source code nya https://github.com/ThonyBiersack/web-sederhana-skillpath-skilvul
4. berikutnya cara menjalankan html dengan manual menggunakan vscode sbb:
        - buat file terlebih dahulu dengan extension nya .html lalu simpan di folder
        - setelah itu isikan file (nama).html tersebut dengan ``` <h1>hello world</h1>``` setelah itu save
        - buka extension di vscode lalu cari live server lalu install live server nya
        - jika sudah restart vscode nya lalu dibagian paling bawah ada go live klik itu
        - jangan lupa install juga live server di google chrome
        - nah nanti bakalan muncul file yang sudah kita buat tadi
5. ada beberapa tag html yang populer yang harus diketahui oleh pemula yaitu
    ### tulisan bold, miring dan garis bawah
        - ```<b>ini tag untuk tulisan bold</b>```
        - ```<i>ini tulisan agar miring</i>```
        - ```<u>tulisan biar ada garis bawah nya</u>
    ### tulisan yang bisa mengarahkan ke link tertentu
        - ```<a href="https://www.wikipedia.org">klik disini</a>```
    ### menampilkan list
        - ```<ol>
                <li>list 1</li>
                <li>list 2</li>
                <li>list 3</li>
            </ol>```
         list diatas untuk menampilkan order list
        - ```<ul>
                <li>list 1</li>
                <li>list 2</li>
                <li>list 3</li>
             </ul>```
          list diatas untuk menampilkan un-order list
    ### tag untuk menyisipkan gambar
        - ```<img src="https://bit.ly/34qGnKk">```
    ### table
        - ```<table>
                <thead>
                    <tr>
                        <th>Mama</th>
                        <th>kota asal</th>
                    </tr>
                 </thead>
                 <tbody>
                    <tr>
                        <td>Thony</td>
                        <td>sukabumi</td>
                    </tr>
                 </tbody>
              </table>```
    ### header & footer
        - ```<header> this is my header</header>```
        - ```<footer> this footer @copyright2022</footer>```
    ### div
        - ```<div>test</div>```
6. apa itu semantic html, menurut saya semantic html itu membuat kerangka html dengan memakai tag yang tersedia dan sesuai.
7. cara mengdeploy project ke github yaitu:
        - login ke netlify kalo belom punya akunya daftar terlebih dahulu
        - lalu ke menu site
        - klik add new site
        - lalu pilih project kalian dari github
        - setelah itu nanti akan di arahkan ke github untuk mengauthorize atau mengkonfirmasi dan memasukan password
        - kemudian sesudah memasukan password pilih project yang akan di deoploy dan kliik deploy
        - lalu web kalian sudah terdeploy.
