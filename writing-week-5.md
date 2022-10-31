# WRITING TEST - WEEK 5
## Web Servers & RESTful API
Web Server merupakan suatu software yang dijalankan di komputer server. Web server adalah suatu perangkat lunak yang mengatur halaman web dan membuat halaman-halaman web tersebut dapat diakses di client, yaitu melalui jaringan lokal atau melalui jaringan Internet. Ada banyak web server yang tersedia diantaranya Apache, IIS Internet Information Service, dan IPlanet’s Enterprise server.

### Server Side Programming
Server side programming atau pemrograman sisi server adalah suatu program yang berjalan di server yang menangani pembuatan konten halaman website yang memiliki fungsi berbeda dengan client side. Pemrograman sisi server merupakan sistem yang berjalan di server, sedang client side merupakan sistem yang berjalan di web browser pengguna. Para pengembang sisi server memiliki tugas untuk merancang, membangun, dan memelihara kode agar sistem dapat berjalan dengan semestinya di server aplikasi. Pemrograman sisi server akan memproses user input, berinteraksi dengan database, dan mengontrol konten apa yang akan disajikan sebagai respon dari permintaan user. Program ini juga bisa membantu meningkatkan pengalaman pengguna dengan cara mengirimkan konten yang sesuai dengan apa yang diinginkan atau diminta oleh user tersebut.

## Nodejs
Node.js adalah runtime environment untuk JavaScript yang bersifat open-source dan cross-platform di mana Node.js merupakan bahasa pemrograman Javascript sisi server yang dibangun di Google Chrome V8 JavaScript Engine. Kelebihan dari Node.js adalah bisa menggunakan Javascript untuk rendering front-end dan menggunakannya kembali di sisi back-end. Node.js sering digunakan para developer untuk mengembangkan konsol, desktop, website, serta web app. Ketika menghandle file request, Node.js bisa menghilangkan proses menunggu sehingga dapat menangani file request selanjutnya dengan cepat.

### Node JS Architecture
Berikut ini adalah beberapa fitur penting dari Node.js yang menjadikannya pilihan utama dalam pengembangan aplikasi:
1. Single Thread<br>
Thread dalam ilmu komputer adalah eksekusi menjalankan beberapa tugas atau program secara bersamaan. Setiap unit yang mampu mengeksekusi kode disebut thread. Javascript menggunakan konsep single thread, yang berarti hanya memiliki satu tumpukan panggilan yang digunakan untuk menjalankan program. Javascript menggunakan call stack untuk melakukan manajemen single thread. Ketika terdapat perintah baru maka akan ditambahkan (push) dan akan di keluarkan ketika perintahnya sudah selasai (pop)
2. Even Loop<br>
Terdapat event queue yang berguna sebagai penampung ketika terdapat perintah baru yang akan dieksekusi. Event loop akan memfasilitasi kondisi ini, event loop akan memeriksa terus menerus, ketika antrian kosong di call stack maka akan menambah antrian baru dari event queue sampai semua perintah selesai di eksekusi.
3. Server Side Scripting<br>
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
1. Console<br>
Console merupakan module bawaan dari javascript yang ada di node JS untuk digunakan sebagai debug atau menampilkan code secara interface
2. Process<br>
Process adalah modules yang digunakan untuk menampilkan dan mengontrol prosess Node JS yang sedang dijalankan.
3. OS<br>
OS module merupakan module yang digunakan untuk menyediakan informasi terkait sistem operasi komputer yang digunakan user.
4. Util<br>
Module Util merupakan alat bantu / utilities untuk mendukung kebutuhan internal API di Node JS
5. Events
6. Errors<br>
Errors merupakan modules yang dapat digunakan untuk mendefinisikan error di Node JS sehingga lebih informatif. Kita juga dapat menghandle error menggunakan try catch
7. Buffer<br>
Buffer merupakan modules yang digunakan untuk mengakses, mengelola dan mengubah tipe data raw atau tipe data bytes
8. Fs<br>
Fs atau “file system” merupakan module yang dapat membantu berinteraksi dengan file yang ada diluar code. FS paling sering digunakan untuk membaca file dengan ekstensi .txt, .csv, dan .json
9. Timers<br>
Timers merupakan modules yang digunakan untuk melakukan scheduling atau mengatur waktu pemanggilan fungsi yang dapat diatur di waktu tertentu

### Membuat Web Server dengan Node JS
* Untuk menggunakan modul HTTP, gunakan require()
* Gunakan method createServer() untuk membuat server HTTP
* Callback function yang digunakan pada method http.createServer(), akan dijalankan ketika seseorang mencoba mengakses komputer pada port 8080.
* Kita bisa menggunakan method res.writeHead() untuk menambahkan header HTTP.
* Argumen pertama dari method res.writeHead() adalah status code, 200 berarti semuanya OK
* Callback function pada method http.createServer() memiliki argumen req yang mewakili request dari klien, sebagai objek (objek http.IncomingMessage).
* Objek ini memiliki sebuah properti yang disebut "url" yang menyimpan informasi url yang sedang mengakses.

## Express Routing & Middleware
Express JS adalah framework dari NodeJS yang dirancang secara fleksibel dan sederhana untuk membantu tahap pengembangan aplikasi back-end. Kelebihan dari framework ini terletak pada fitur caching, support dengan Google V8 Engine, JavaScript, serta didukung oleh komunitas dan skalabilitas aplikasi yang baik.

### REST API
RESTful API / REST API merupakan penerapan dari API (Application Programming Interface). Sedangkan REST (Representional State Transfer) adalah sebuah arsitektur metode komunikasi yang menggunakan protokol HTTP untuk pertukaran data dimana metode ini sering diterapkan dalam pengembangan aplikasi. Dengan tujuannya untuk menjadikan sistem memiliki performa yang baik, cepat dan mudah untuk di kembangkan (scale) terutama dalam pertukaran dan komunikasi data.<br>

RESTFUL API memiliki 4 komponen penting yaitu:
1. URL Design
2. HTTP Verbs
3. HTTP Response Code
4. Format Response

### Basic Routes
1. Routes<br>
Routes adalah sebuah end point yang diapat kita akses menggunakan URL di website. Didalam routes kita perlu menentukan method API, alamat dan response apa saja yang akan dikeluarkan.
2. method<br>
Kita dapat menggunakan method yang dalam REST API seperti POST, PUT, PATCH dan DELETE.
3. Response<br>
Di dalam route kita dapat mengirim response menggunakan parameter dari route express.js yaitu “res.Send()” untuk mengirim plain text ketika kita mengakses route tersebut. Kita dapat mengirim response berupa output json yang biasa dipakai untuk back end application. Dengan menggunakan output json maka kita dapat mengirim data yang mudah diakses.
4. Status Code<br>
Dalam pengaplikasian back end application, kita sangat perlu memberikan status code sebagai informasi apakah route yang kita akses berjalan sebagaimana mestinya dan tidak terjadi error.
5. Query<br>
Query merupakan parameter yang digunakan untuk membantu menentukan tindakan yang lebih spesifik daripada hanya sekedar router biasa. 
6. Nested Route<br>
Nested route digunakan ketika terdapat banyak route yang memiliki nama yang sama atau ingin membuat route yang lebih mendalam.

### Express Middleware
Middleware function adalah sebuah fungsi yang memiliki akses ke object request (req), object response (res), dan sebuah fungsi next didalam request-response cycle.

Pada dasarnya, sebuah middleware function dapat melakukan tugas-tugas berikut:<br>
* Menjalankan kode apapun.
* Memodifikasi Object Request dan Object Response.
* Menghentikan request-response cycle.
* Melanjutkan ke middleware function selanjutnya atau ke handler function dalam suatu request response cycle.

Jenis Express Middleware Berdasarkan Cara Penggunaan<br>
1. Application Level Middleware<br>
* Application Level Middleware adalah sebuh function middleware yang melekat ke instance object Application Express.
* Penggunaannya dengan cara memanggil method app.use().
* Application Level Middleware akan di jalankan setiap kali Express Application menerima sebuah HTTP Request.
```
const addRequestTime = function (req, res, next)
{
    req.requestTime = Date.now()
    next()
}
app.use(addRequestTime)
```
2. Router Level Middleware<br>
* Router Level Middleware adalah sebuh function middleware yang cara kerjanya sama persis dengan application level middleware, yang menjadikan perbedaan adalah middleware function ini melekat ke instance object Router Express.
* Penggunaannya dengan cara memanggil method express.Router().
* Router Level Middleware hanya akan di jalankan setiap kali sebuah Express Router yang menggunakan middleware ini menerima sebuah HTTP Request, sedangan pada Router yang lain tidak akan dijalankan.
3. Error Handling Middleware<br>
* Error Handling mengacu kepada bagaimana cara sebuah Express Application menangkap dan memproses error yang terjadi, baik itu berupa kesalahan yang synchronous maupun asynchronous.
* Express Application sudah menyediakan error handle function default, sehingga kita tidak perlu lagi membuat sendiri functionnya.
* Error handle function default milik Express Application hanyalah kerangka functionnya saja, kita tetap harus menuliskan di dalam function ini bagaimana sebuah error akan di handle.
* Error Handling Middleware digunakan pada Application Level Middleware
```
const express = require("express")
const app = express()

const errorHandling = function(err, req, res, next){
    console.error(err.stack)
    res.status(500).send('Something broke!')
}
app.use(errorHandling)
```

Jenis Express Middleware Berdasarkan Source Middleware Function<br>
1. Express Build-in Middleware
* express.static()
* express.json()
* express.urlEncoded()
2. Third Party (custom) Middleware
* cors
* body-parser
* errorhandler
* morgan
* Multer

## Design Database with MySQL
Menentukan Entity & Attributes<br>
1. Identifikasi entity dalam database.
2. List entity yang ada.
3. Pada tahap menentukan Atrributes, tentukan attributes apa saja yang datanya akan disimpan di dalam sebuah entity.
4. Attributes yang diperlukan didalam entity kemungkinan sudah ada di dalam requirements document, atau mungkin juga diperlukan penafsiran kita sendiri sebagai database developer.

