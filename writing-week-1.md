# WRITING TEST - WEEK 1
## Git & Github Dasar
Git merupakan sebuah tools berbasis Version Control System yang biasa digunakan oleh programmer dan developer untuk menjalankan proyek pengembangan software. Git bertugas untuk mencatat setiap perubahan yang terjadi pada file atau repository suatu project. Git biasanya digunakan oleh para programmer sebagai tempat penyimpanan file pemrograman karena lebih efektif. File-file yang disimpan menggunakan git akan terlacak seluruh perubahannya, termasuk siapa yang mengubah. Dengan menggunakan Git dan Github, dapat mempermudah berkolaborasi dalam sebuah tim untuk mengerjakan proyek yang sama. 

1. Instalasi Git dan Setup Awal
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

## Basic Git Command
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

## Perintah Dasar CLI (Command Line Interface)
* pwd (print working directory) untuk melihat direktori di mana kita berada.
* ls (lists) untuk melihat isi dari direktori.
* cd (change directory) untuk pindah ke direktori lain.
* touch untuk membuat file
* mkdir untuk membuat direktori
* head untuk melihat beberapa line awal dari sebuah file text
* tail untuk melihat beberapa line awal dari sebuah file text
* cat untuk melihat isi sebuah file
* cp untuk menyalin file atau direktori
* mv untuk memindahkan dan mengubah nama file atau direktori.
* rm untuk menghapus file atau direktori.

## HTML
HTML (Hypertext Markup Language) adalah bahasa markup yang digunakan untuk membuat halaman website dan menampilkan konten pada browser. Konten yang dapat ditampilkan dapat berupa Text, Image, Video, Link, dan masih banyak lainnya. Untuk membuat HTML diperlukan 2 tools, yaitu browser dan code editor. Visual Studio Code adalah salah satu code editor yang dikembangkan oleh tim engineer Microsoft. Keunggulan Visual Studio Code dapat digunakan di Windows, Mac, dan juga Linux. HTML dapat dijalankan secara manual pada browser atau menggunakan ekstensi live server pada Visual Studio Code.

Tag-tag dasar pada HTML:
<!DOCTYPE html> — untuk deklarasi tipe dokumen.
<html> — tag utama dalam HTML.
<head> — untuk bagian kepala dari dokumen.
<title> — untuk judul web.
<body> — untuk bagian body dari dokumen.

## CSS
CSS atau Cascading Style Sheets adalah kumpulan perintah yang digunakan untuk menjelaskan tampilan sebuah halaman situs web dalam mark-up language. CSS berfungsi untuk menjelaskan dan menata tampilan elemen yang tertulis pada bahasa markup, salah satunya adalah HTML. Sintaks CSS terdiri dari 3 bagian yaitu selector, property, value. 

Terdapat 3 cara untuk menyisipkan CSS ke dalam HTML di antaranya:
1. Inline CSS, dengan menambahkan CSS menggunakan atribut style pada tag pembuka elemen HTML.
``` <p style="padding: 10px; background-color: blue;">Inline CSS</p> ```
2. Internal CSS, dengan menambahkan CSS menggunakan tag <style> di dalam tag <head>.
``` <style></style> ```
3. External CSS, menambahkan CSS di luar dokumen HTML dan dihubungkan dengan menggunakan tag <link> di dalam elemen <head> yang didefinisikan pada setiap dokumen HTML.

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