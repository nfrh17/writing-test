# WRITING TEST - WEEK 1
## Git & Github Dasar
Git merupakan sebuah tools berbasis Version Control System yang biasa digunakan oleh programmer dan developer untuk menjalankan proyek pengembangan software. Git bertugas untuk mencatat setiap perubahan yang terjadi pada file atau repository suatu project. Git biasanya digunakan oleh para programmer sebagai tempat penyimpanan file pemrograman karena lebih efektif. File-file yang disimpan menggunakan git akan terlacak seluruh perubahannya, termasuk siapa yang mengubah. Dengan menggunakan Git dan Github, dapat mempermudah berkolaborasi dalam sebuah tim untuk mengerjakan proyek yang sama. 

1. Instalasi Git dan Setup Awal<br>
Untuk mengecek apakah instalasi berhasil dapat dilakukan
``` 
git –version 
```

Setelah itu lakukan setup awal pada git 
``` 
git config –global user.name “nama”
git config –global user.email “contoh@email.com”
```

Untuk mengecek apakah setup awal telah berhasil dapat dilakukan
``` 
git config –list 
```

2. Basic Git Command
* git status, digunakan untuk menampilkan daftar file yang berubah bersama dengan file yang ingin ditambahkan atau di-commit.
* git init namaproject, untuk membuat repository
* git add, digunakan untuk menambahkan file baru di repository yang dipilih.
* git commit -m “pesan”, digunakan untuk melakukan commit pada perubahan yang dilakukan.
* git remote, untuk membuat user terhubung ke remote repository.
* git push, untuk mengirimkan perubahan ke master branch dari remote repository. yang berhubungan dengan direktori lokal.
* git clone digunakan untuk membuat salinan repository lokal.

## Unix Command Line
* Shell, program yang digunakan untuk berkomunikasi atau memerintah sistem
* Command Line Interface, jenis shell yang berbasis teks
* Terminal Emulator adalah aplikasi untuk mengakses CLI

#### Perintah Dasar CLI (Command Line Interface)
* pwd (print working directory) untuk melihat direktori di mana kita berada.
* ls (lists) untuk melihat isi dari direktori.
* cd (change directory) untuk pindah ke direktori lain.
* touch untuk membuat file.
* mkdir untuk membuat direktori.
* head untuk melihat beberapa line awal dari sebuah file text.
* tail untuk melihat beberapa line awal dari sebuah file text.
* cat untuk melihat isi sebuah file.
* cp untuk menyalin file atau direktori.
* mv untuk memindahkan dan mengubah nama file atau direktori.
* rm untuk menghapus file atau direktori.

## HTML
HTML (Hypertext Markup Language) adalah bahasa markup yang digunakan untuk membuat halaman website dan menampilkan konten pada browser. Konten yang dapat ditampilkan dapat berupa Text, Image, Video, Link, dan masih banyak lainnya. Untuk membuat HTML diperlukan 2 tools, yaitu browser dan code editor. Visual Studio Code adalah salah satu code editor yang dikembangkan oleh tim engineer Microsoft. Keunggulan Visual Studio Code dapat digunakan di Windows, Mac, dan juga Linux. HTML dapat dijalankan secara manual pada browser atau menggunakan ekstensi live server pada Visual Studio Code.

Tag-tag dasar pada HTML:
1. ```<!DOCTYPE html>``` — untuk deklarasi tipe dokumen.
2. ```<html>``` — tag utama dalam HTML.
3. ```<head>``` — untuk bagian kepala dari dokumen.
4. ```<title>``` — untuk judul web.
5. ```<body>``` — untuk bagian body dari dokumen.

Semantik pada HTML adalah elemen-elemen yang menyatakan makna atau tujuan dari elemen itu sendiri. Salah satu keuntungan menggunakan elemen semantik adalah dokumen HTML akan mudah dibaca, baik itu oleh manusia maupun mesin.

Berikut adalah daftar elemen-elemen semantik:
* ```<article>```  untuk membuat elemen artikel.
* ```<aside>```  untuk membuat elemen bagian samping.
* ```<details>```  untuk membuat elemen datail.
* ```<figcaption>```  untuk membuat teks caption pada figure.
* ```<figure>```  untuk membuat figur atau gambar pada artikel.
* ```<footer>```  untuk membuat elemen bagian kaki dari web.
* ```<header>```  untuk mebuat kepala kop dari web.
* ```<main>```  untuk membuat elemen utama.
* ```<mark>```  untuk menandai teks.
* ```<nav>```  untuk membuat navigasi.
* ```<section>```  untuk membuat bagian artikel.
* ```<summary>```  untuk membuat ringkasan artikel.
* ```<time>```  untuk membuat elemen yang menyatakan waktu

Contoh semantik HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Contoh Elemen Semantik</title>
</head>
<body>
  <header>
    <h1>Semantic HTML</h1>
  </header>
  <nav>
    <a href="#">Home</a> |
    <a href="#">About</a> |
    <a href="#">Contact</a>
  </nav>
  <article>
    <h1>Ini adalah kode semantik HTML</h1>
    <p>Semantik elemen bertujuan agar dokumen HTML mudah dibaca.</p>
  </article>
  <footer>
    Copyright ``` &copy; ``` 2020
  </footer>
</body>
</html>
```

Deployment adalah kegiatan yang bertujuan untuk menyebarkan aplikasi yang telah dikerjakan. Kita dapat mendeploy HTML dengan menggunakan Netlify.

## CSS
CSS atau Cascading Style Sheets adalah kumpulan perintah yang digunakan untuk menjelaskan tampilan sebuah halaman situs web dalam mark-up language. CSS berfungsi untuk menjelaskan dan menata tampilan elemen yang tertulis pada bahasa markup, salah satunya adalah HTML. Sintaks CSS terdiri dari 3 bagian yaitu selector, property, value. 

Terdapat 3 cara untuk menyisipkan CSS ke dalam HTML di antaranya:
1. Inline CSS, dengan menambahkan CSS menggunakan atribut style pada tag pembuka elemen HTML.
``` 
<p style="padding: 10px; background-color: blue;">Inline CSS</p> 
```
2. Internal CSS, dengan menambahkan CSS menggunakan tag ```<style>``` di dalam tag ```<head>```.
``` 
<style></style> 
```
3. External CSS, menambahkan CSS di luar dokumen HTML dan dihubungkan dengan menggunakan tag ```<link>``` di dalam elemen ```<head>``` yang didefinisikan pada setiap dokumen HTML.

## Algoritma & Pseudocode
Algoritma adalah deskripsi berupa step-step yang dibutuhkan untuk menyelesaikan suatu masalah. Bagi programmer, algoritma akan memudahkan mereka melakukan tracking kesalahan-kesalahan (error) yang timbul.

Ciri dari Algoritma:
* tidak ambigu, tiap tahap hanya punya satu makna
* ada input, minimal 0, bisa lebih
* ada output, minimal 1, bisa lebih
* ada batas jumlah langkah
* layak, sesuai dengan sumber daya yang ada
* independen, tidak bergantung bahasa pemrograman tertentu
* efektif dan efisien, satu tahap bersifat sederhana dan punya batas waktu

Pseudocode adalah menuliskan algoritma dengan umumnya bahasa inggris sebelum kita implementasikan ke bahasa pemrograman tertentu. Tujuan dari penggunaan pseudocode adalah untuk mempermudah manusia dalam menyelesaikan suatu permasalahan yang dihadapi.

Ciri dari Pseudocode:
* Pseudocode adalah notasi atau tanda bagaimana cara menyelesaikan masalah dengan sistematis dan runut.
* Pseudocode digunakan untuk menulis algoritma.
* Pseudocode berisikan serangkaian proses untuk menyelesaikan permasalahan.
* Bahasa yang digunakan lebih ringkas serta mudah dipahami.
* Tidak memiliki aturan baku dalam menuliskan pseudocode.

## Javascript
Javascript adalah bahasa pemrograman yang digunakan dalam pengembangan website untuk membuat interaksi pada website agar lebih dinamis. Website dinamis yang dimaksud berarti konten di dalamnya dapat bergerak atau mengubah apapun yang tampak di layar tanpa harus dimuat ulang secara manual. Misalnya seperti konten gambar animasi, maps, slideshow, polling, dan sebagainya.

### Tipe data
1. Null, tipe data primitive yang nilainya null.
2. Undefined, tipe data primitive yang nilainya undefined atau tidak terdefinisikan.
3. Boolean, tipe data yang hanya memiliki dua nilai, yakni true dan false.
4. Number, tipe data yang mewakili seluruh tipe data angka, seperti integer (bilangan bulat) dan floating point atau desimal.
5. String, tipe data yang berhubungan dengan karakter.
6. Symbol, merupakan tipe data baru setelah hadirnya ECMAScript 6 (ES6).
7. NaN, adalah nilai numeric yang spesial. Digunakan untuk memberitahu bahwa nilai dari variabel tersebut adalah invalid number atau bukan termasuk angka.
8. Object, merupakan tipe data kompleks yang berisi kumpulan properti (props), setiap properti berisi pasangan key:value.

### Variabel
Variabel adalah container yang digunakan untuk menyimpan sebuah nilai. Terdapat 3 cara untuk mendefinisikan variabel pada Javascript, yaitu var, let, dan const. Untuk menampilkan isi variabel, bisa digunakan fungsi-fungsi berikut:
* console.log() menampilkan output ke console javascript;
* document.write() menampilkan output ke dokumen HTML;
* alert() menampilkan output ke jendela dialog.

### Operator Pada Javascript
Operator adalah instruksi yang digunakan untuk suatu proses.
1. Operator Aritmatika
* Penjumlahan(+), menjumlahkan 2 operand
* Pengurangan(-), mengurangi suatu operand dengan operand lainnya
* Perkalian(*), mengalikan suatu operand dengan operand yang lainnya
* Pembagian(/), operasi pembagian: suatu operand akan dibagi dengan operand lainnya
* Modulus(%), menghasilkan sisa bagi dari hasil pembagian suatu operand dengan operand lainnya
* Increment(++), menambah 1 nilai keatas pada operand/variabel
* Decrement(--), mengurangi 1 nilai kebawah pada operand/variabel

2. Operator Perbandingan
* Equal(==)	TRUE jika kedua operand nilainya sama
* Not Equal(!=)	TRUE jika kedua operand nilainya tidak sama
* Identical(===)	TRUE jika kedua operand nilainya sama dan dengan tipe data yang sama
* Not Identical(!==)	TRUE jika ke-2 operand nilainya tidak sama serta bertipe data berbeda
* Lebih Besar(>)	TRUE jika suatu operand nilainya lebih besar dari operand lainnya.
* Lebih Kecil(<)	TRUE jika suatu operand nilainya lebih kecil dari operand lainnya
* Lebih Besar sama dengan(>=)	TRUE jika operand pertama nilainya lebih besar atau sama, dengan operand kedua
* Lebih Kecil sama dengan(>=)	TRUE jika operand pertama nilainya lebih kecil atau sama, dengan operand kedua

3. Operator Logika
* and(&&)	TRUE jika kedua operand nilainya cocok, benar(true), misal true && true
* or(||)	TRUE jika salah satu dari kedua operand bernilai Benar(true).
* not(!)	TRUE jika nilai dari kedua operand tidak cocok

### Percabangan Pada Javascript
1. if<br>
Percabangan if merupakan percabangan yang hanya memiliki satu blok pilihan saat kondisi bernilai benar.
2. if-else<br>
if-else merupakan percabangan yang memiliki dua blok pilihan.
```
if (kondisi){
    // blok kode
}
else {
    //blok kode
}
```
3. switch-case
```
switch(variabel){
    case <value>:
        // blok kode
        break;
    case <value>:
        // blok kode
        break;
    default:
        // blok kode
}
```

### Perulangan Pada Javascript
1. For Loop
``` 
for ([initialExpression]; [condition]; [incrementExpression]) statement;
```
2. While<br>
Pada while loop, perulangan terus dilakukan selama kondisi awal bernilai true.
```
while (condition) statement;
```
3. Do While<br>
Pada do while, perulangan terus dilakukan sampai kondisi bernilai false.
```
do
  statement
while (condition);
```