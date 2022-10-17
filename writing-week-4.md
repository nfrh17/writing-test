# WRITING TEST - WEEK 4
## Git & Github Lanjutan
Git adalah aplikasi yang dapat melacak setiap perubahan yang terjadi pada suatu folder atau file. File -file yang disimpan menggunakan git akan terlacak seluruh perubahannya, termasuk siapa yang mengubah. Dengan menggunakan GIT dan Github, kamu akan bisa bekerja dalam sebuat tim. Tujuan besarnya adalah kamu bisa berkolaborasi mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate.

#### Cara berkolaborasi dengan tim menggunakan Github
* git init, untuk menghubungkan folder tersebut dengan git (jika sudah terhubung dengan biasa terdapat tulisan nama branch seperti master)
* git remote add origin, untuk menhubungkan folder dengan github
* git add, untuk menambahkan file baru di repository yang dipilih.
* git commit -m "message", untuk mengupload perubahan tersebut ke git (masih local)
* git push -u origin main, untuk mengupload perubahan tersebut ke github
* Agar file sinkron antara github dan yang ada di local maka gunakan perintah git pull origin master
* Untuk menghindari conflict code yang dikembangkan, kita tidak boleh berkolaborasi dalam project di satu branch yang sama
* Dalam berkolaborasi, setiap fitur harus dibuat branch masing-masing dengan perintah git branch <branch>
* Git merge, untuk menyatukan branch cabang fitur yang telah kita kembangkan

## Responsive Web
Responsive Web Design (RWD) bertujuan untuk membuat desain website kita dapat diakses dalam device apapun. Setiap developer website wajib menggunakan tools bawaan dari setiap browser yang memudahkan proses development website.

1. Menambahkan viewport di dalam HTML
```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
2. Gunakan elemen max-width
3. Gunakan media query
Media query digunakan untuk membuat beberapa styles tergantung pada jenis device. Media query untuk responsive web design umumnya hanya menggunakan 2 jenis media query, yaitu min-width dan max-width

## Bootstrap
Bootstrap adalah framework HTML, CSS, dan JavaScript yang berfungsi untuk mendesain website responsive dengan cepat dan mudah. Framework open source ini diciptakan pada tahun 2011 oleh Mark Otto dan Jacob Thornton dari Twitter. Itulah kenapa dulunya Bootstrap dinamakan Twitter Blueprint.