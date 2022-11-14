# WRITING TEST - WEEK 7
## Sequelize
Sequelize adalah ORM Node JS yang berbasis promise. Sequelize bisa digunakan dengan PostgreSQL, MySQL, MariaDB, SQLite, dan MSSQL. Dengan fitur fitur di Sequelize, kita bisa mengelola dan mengatur data di database kita dengan cepat, dan efisien.

## MongoDB
MongoDB adalah salah satu database open source NoSQL yang cukup populer digunakan. MongoDB sering dipakai untuk aplikasi berbasis Cloud, Big Data maupun Grid Computing. MongoDB menyimpan data menggunakan dokumen dengan format JSON. MongoDB termasuk database NoSQL yang berarti kita bisa mengolah database dengan fleksibel dan tidak membutuhkan Query.

Kelebihan:
* Sistem tidak membutuhkan Tabel
* Tidak perlu menggunakan Tabel yang terstruktur
* By Default sudah menggunakan JSON(JavaScript Object Notation), sehingga memudahkan integrasi dengan JavaScript
* Performa lebih cepat dengan kemampuan menampung banyak data yang bervariasi

Kekurangan:
* Tidak mendukung transaksi
* Masalah konsistensi data
* Menggunakan banyak memory
* Hanya bisa menampung maksimal 16MB disetiap document

## Mongoose
Mongoose adalah library yang bisa dibilang sebagai Object Modelling MongoDB untuk NodeJS. Mongoose bisa digunakan untuk mengelola hubungan antara data, menyediakan validasi. Moongose juga bisa digunakan untuk menerjemahkan antara objek dalam kode dan representasi Objek tersebut di MongoDB. 

## Docker
Docker adalah software yang menjalankan suatu aplikasi menggunakan container. Docker men-sharing kernel dari host OS, serta meng-container-kan suatu aplikasi agar dapat dijalankan dimana saja dan kapan saja. Docker berfungsi sebagai penyedia layanan virtual bagi aplikasi yang diinstall pada sebuah host. Docker akan menyediakan hal-hal yang diperlukan untuk aplikasi mulai dari akses file, koneksi internet, hingga port agar aplikasi dapat berjalan dengan mulus.

Perintah Dasar Docker:
1. docker pull, untuk download image dari docker hub.
2. docker images, untuk melihat kumpulan images yang sudah terdownload.
3. docker run, menjalankan container.
4. docker ps, untuk melihat container yang berjalan.

### Docker File
Docker File merupakan sebuah blueprint untuk  membuat image, kamu juga bisa membuat custom image menggunakan docker file.

Caranya:
1. Buat file Dockerfile di dalam project yang kamu buat
2. Tulis beberapa perintah ke dalam dockerfile
3. Jalankan docker file menggunakan perintah 
```
docker build -t NAMA_IMAGES:TAG . 
docker build -t my-app:1.0 . 
```