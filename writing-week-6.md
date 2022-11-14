# WRITING TEST - WEEK 6
## MySQL Lanjutan
### Relations di SQL
1. One to Many, merupakan relasi yang paling sering digunakan. Satu baris dalam tabel dapat memiliki beberapa baris di tabel relasinya.
2. Many to Many, digunakan ketika kedua tabel yang berelasi dapat memiliki beberapa baris di tabel relasinya.
3. One to One, merupakan relasi yang sangat jarang digunakan. Diimplementasikan dengan cara yang sama seperti One to Many tetapi dengan kondisi tambahan (foreign key merupakan primary key).

### Database Normalization
Database Normalization merupakan teknik analisis data yang mengorganisasikan atribut-atribut data dengan cara mengelompokkan sehingga terbentuk entitas yang non-redundant, stabil, dan fleksible. Tujuannya antara lain menghilangkan redundan data pada database, memudahkan juka ada perubahan struktur table database, dan memperkecil pengaruh jika ada perubahan dari struktur tabel database.

### Key di SQL
1. Super Key, merupakan kumpulan dari satu atau lebih dari satu key yang dapat digunakan untuk mengidentifikasi record secara unik dalam sebuah tabel. Super Key adalah superset dari Candidate Key.
2. Candidate Key, merupakan kumpulan satu atau lebih fields/columns yang dapat mengidentifikasi record secara unik dalam tabel. Bisa jadi ada beberapa Candidate Keys di dalam satu tabel. Setiap Candidate Key bisa digunakan sebagai Primary Key. Candidate Key adalah super key yang tidak mempunyai value yang berulang.
3. Primary Key, merupakan kumpulan satu atau lebih fields/columns dari sebuah tabel yang secara unik mengidentifikasi sebuah record dalam tabel database. Valuenya tidak boleh berupa null ataupun duplicate value. Hanya boleh salah satu Candidate Key yang bisa menjadi Primary Key.
4. Alternate Key, key yang bisa digunakan menjadi primary key. Pada dasarnya, Key ini merupakan candidate key yang tidak dijadikan  primary key.
5. Unique Key, merupakan kumpulan dari satu atau lebih fields/columns di sebuah table database yang secara unik mengidentifikasi sebuah record dalam table database tersebut. Hampir sama dengan Primary key, namun value dari Unique Key bisa berupa satu buah null value di dalam sebuah table database, dan Unique Key tidak bisa memiliki duplicate values.
6. Foreign Key, merupakan field di sebuah table database yang menjadi Primary Key di table database lain. Value dari Foreign key bisa menerima multiple null dan duplicate values.

### Join Multiple Tables
Untuk mengambil records dari dua atau lebih table database yang memiliki relationship dan akan di sajikan dalam single result set.
1. INNER JOIN, semua baris akan diambil dari kedua tabel yang akan di JOIN, selama columns cocok dengan kondisi yang sudah di tentukan.
2. LEFT JOIN, semua records dari table di sisi kiri JOIN statement akan di pilih.
3. RIGHT JOIN, semua records dari table di sisi kiri JOIN statement akan di pilih, bahkan jika table di sebelah kiri tidak memiliki record yang cocok.

## Authentication & Authorization
* Authentication merupakan proses memverifikasi user untuk mendapatkan hak akses.
* Authorization proses lanjutan setelah proses authentication yaitu menilai apa sajakah layanan yang dapat dinikmati pengguna yang sudah jelas identitasnya (authenticated user). Dalam proses authorization, akun kembali diperiksa apakah memiliki izin untuk mengakses resource yang dimaksud. Jika memiliki izin, maka request akan dilanjutkan, namun apabila tidak memiliki izin, maka request akan dibatalkan. Dalam hal ini biasanya server akan mengembalikan status 403 Forbidden ke browser yang artinya akses tidak diizinkan.

## Sequelize
Sequelize adalah ORM (Object Relational Mapping) Node JS yang berbasis promise. Sequelize mendukung sebagian besar relational Database seperti MySQL, PostgresQL, MariaDB, SQLite, dan Microsoft SQL Server. ORM itu sendiri merupakan suatu metode/teknik pemrograman yang digunakan untuk mengkonversi data dari lingkungan bahasa pemrograman berorientasi objek (OOP) dengan lingkungan database relational.  