# WRITING TEST - WEEK 5
## Web Servers & RESTful API
Web Server merupakan suatu software yang dijalankan di komputer server. Web server adalah suatu perangkat lunak yang mengatur halaman web dan membuat halaman-halaman web tersebut dapat diakses di client, yaitu melalui jaringan lokal atau melalui jaringan Internet. Ada banyak web server yang tersedia diantaranya Apache, IIS Internet Information Service, dan IPlanet’s Enterprise server.

### Server Side Programming
Server side programming atau pemrograman sisi server adalah suatu program yang berjalan di server yang menangani pembuatan konten halaman website yang memiliki fungsi berbeda dengan client side. Pemrograman sisi server merupakan sistem yang berjalan di server, sedang client side merupakan sistem yang berjalan di web browser pengguna. Para pengembang sisi server memiliki tugas untuk merancang, membangun, dan memelihara kode agar sistem dapat berjalan dengan semestinya di server aplikasi. Pemrograman sisi server akan memproses user input, berinteraksi dengan database, dan mengontrol konten apa yang akan disajikan sebagai respon dari permintaan user. Program ini juga bisa membantu meningkatkan pengalaman pengguna dengan cara mengirimkan konten yang sesuai dengan apa yang diinginkan atau diminta oleh user tersebut.

### Static Web Server


## Nodejs
Node.js adalah runtime environment untuk JavaScript yang bersifat open-source dan cross-platform di mana Node.js merupakan bahasa pemrograman Javascript sisi server yang dibangun di Google Chrome V8 JavaScript Engine. Kelebihan dari Node.js adalah bisa menggunakan Javascript untuk rendering front-end dan menggunakannya kembali di sisi back-end. Node.js sering digunakan para developer untuk mengembangkan konsol, desktop, website, serta web app. Ketika menghandle file request, Node.js bisa menghilangkan proses menunggu sehingga dapat menangani file request selanjutnya dengan cepat.

### Node JS Architecture
Berikut ini adalah beberapa fitur penting dari Node.js yang menjadikannya pilihan utama dalam pengembangan aplikasi:
1. Single Thread
Thread dalam ilmu komputer adalah eksekusi menjalankan beberapa tugas atau program secara bersamaan. Setiap unit yang mampu mengeksekusi kode disebut thread. Javascript menggunakan konsep single thread, yang berarti hanya memiliki satu tumpukan panggilan yang digunakan untuk menjalankan program. Javascript menggunakan call stack untuk melakukan manajemen single thread. Ketika terdapat perintah baru maka akan ditambahkan (push) dan akan di keluarkan ketika perintahnya sudah selasai (pop)
2. Even Loop
Terdapat event queue yang berguna sebagai penampung ketika terdapat perintah baru yang akan dieksekusi. Event loop akan memfasilitasi kondisi ini, event loop akan memeriksa terus menerus, ketika antrian kosong di call stack maka akan menambah antrian baru dari event queue sampai semua perintah selesai di eksekusi.
3. Server Side Scripting
Dengan menggunakan NodeJS kita dapat menjalankan javascript di server side menggunakan terminal command line menggunakan perintah ``node``.

### Arrow Expression
Arrow expression merupakan fitur terbaru dari javascript, yaitu mempermudah membuat sintaks function menggunakan “=>” 
```
//non arrow function
function countLength(val1, val2) {
    return val1.length + val2.length
}
//using arrow function
const countLengthChar = (val1, val2) => return val1.length + val2.length
```

### Asynchronous
Asynchronous merupakan konsep yang paling penting dari javascript. Pada dasarnya, javascript mengeksekusi code secara single thread dan berurutan baris per baris yang disebut dengan synchronous. Sedangkan asynchronous memungkinkan mengeksekusi code tanpa berurutan dengan cara “skip” code dan melanjutkan eksekusi code selanjutnya. Konsep ini menungkinkan code kita tidak terjadi blocking dan lebih efisien.
```
console.log('Hello');
setTimeout(() => { console.log('Javascript')},100)
console.log('Coder');
```

### JSON
JSON atau Javascript Object Notation merupakan format yang digunakan untuk menyimpan dan mengirim data menggunakan konsep object di javascript. JSON dapat digunakan di hampir semua bahasa pemrograman sehingga sangat cocok untuk dipelajari.
```
{"users": [
    {"username" : "Anton", "lokasi" : "Bandung"},
    {"username" : "Budi", "lokasi" : "Semarang"},
    {"username" : "Nana", "lokasi" : "Surabaya"},
    {"username" : "Jamal", "lokasi" : "Tangerang"},
]}
```

### Build in Module Node JS
1. Console
Console merupakan module bawaan dari javascript yang ada di node JS untuk digunakan sebagai debug atau menampilkan code secara interface
2. Process
Process adalah modules yang digunakan untuk menampilkan dan mengontrol prosess Node JS yang sedang dijalankan.
3. OS
OS module merupakan module yang digunakan untuk menyediakan informasi terkait sistem operasi komputer yang digunakan user.
4. Util
Module Util merupakan alat bantu / utilities untuk mendukung kebutuhan internal API di Node JS
5. Events
6. Errors
Errors merupakan modules yang dapat digunakan untuk mendefinisikan error di Node JS sehingga lebih informatif. Kita juga dapat menghandle error menggunakan try catch
7. Buffer
Buffer merupakan modules yang digunakan untuk mengakses, mengelola dan mengubah tipe data raw atau tipe data bytes
8. Fs
Fs atau “file system” merupakan module yang dapat membantu berinteraksi dengan file yang ada diluar code. FS paling sering digunakan untuk membaca file dengan ekstensi .txt, .csv, dan .json
9. Timers
Timers merupakan modules yang digunakan untuk melakukan scheduling atau mengatur waktu pemanggilan fungsi yang dapat diatur di waktu tertentu

### Membuat Web Server dengan Node JS
* Untuk menggunakan modul HTTP, gunakan require()
* Gunakan method createServer() untuk membuat server HTTP
* Callback function yang digunakan pada method http.createServer(), akan dijalankan ketika seseorang mencoba mengakses komputer pada port 8080.
* Kita bisa menggunakan method res.writeHead() untuk menambahkan header HTTP.
* Argumen pertama dari method res.writeHead() adalah status code, 200 berarti semuanya OK

## Express Routing & Middleware

## Design Database with MySQL