# WRITING TEST - WEEK 5
## MySQL Lanjutan
### Relations in MySQL
1. One to Many, merupakan relasi yang paling sering digunakan. Satu baris dalam tabel dapat memiliki beberapa baris di tabel relasinya.
2. Many to Many, digunakan ketika kedua tabel yang berelasi dapat memiliki beberapa baris di tabel relasinya.
3. One to One, merupakan relasi yang sangat jarang digunakan. Diimplementasikan dengan cara yang sama seperti One to Many tetapi dengan kondisi tambahan (foreign key merupakan primary key).

### Database Normalization
Database Normalization merupakan teknik analisis data yang mengorganisasikan atribut-atribut data dengan cara mengelompokkan sehingga terbentuk entitas yang non-redundant, stabil, dan fleksible. Tujuannya antara lain menghilangkan redundan data pada database, memudahkan juka ada perubahan struktur table database, dan memperkecil pengaruh jika ada perubahan dari struktur tabel database.

## Authentication & Authorization
* Authentication merupakan proses memverifikasi user untuk mendapatkan hak akses.
* Authorization proses lanjutan setelah proses authentication yaitu menilai apa sajakah layanan yang dapat dinikmati pengguna yang sudah jelas identitasnya (authenticated user). Dalam proses authorization, akun kembali diperiksa apakah memiliki izin untuk mengakses resource yang dimaksud. Jika memiliki izin, maka request akan dilanjutkan, namun apabila tidak memiliki izin, maka request akan dibatalkan. Dalam hal ini biasanya server akan mengembalikan status 403 Forbidden ke browser yang artinya akses tidak diizinkan.

## Sequelize
Sequelize adalah ORM (Object Relational Mapping) Node JS yang berbasis promise. Sequelize mendukung sebagian besar relational Database seperti MySQL, PostgresQL, MariaDB, SQLite dan Miscrosoft SQL Server. ORM itu sendiri merupakan suatu metode/teknik pemrograman yang digunakan untuk mengkonversi data dari lingkungan bahasa pemrograman berorientasi objek (OOP) dengan lingkungan database relational.  