# WRITING TEST - WEEK 2
## Scope
Scope adalah konsep dalam flow data variabel. Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak. Terdapat tiga jenis scope dalam Javascript, yaitu global scope, local scope, dan block scope.
1. Block Scope
Blocks adalah code yang berada didalam curly braces {}. Pada conditional, function, dan looping menggunakan blocks.
2. Global Scope
Global scope berarti variabel yang kita buat dapat diakses dan dimodifikasi dimanapun dalam suatu file. Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar blocks. Variabel yang dideklarasikan dalam global scope biasa disebut variabel global.
Contoh global scope:
```
let myName = 'Raisha';

function greeting() {
    return myName; // Raisha
}

console.log(myName); // Raisha
```
3. Local Scope
Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping. Maka variabel hanya bisa diakses didalam blocks saja, tidak bisa diakses diluar blocks.

Contoh local scope:
```
// Variable declare in function blocks
function greeting() {
    let myName = 'Raisha';
    return myName; // Raisha
}

console.log(greeting()) // Raisha
console.log(myName); // Uncaught ReferenceError: myName is not defined because local scope
```

## Function
Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task atau 1 fitur. Dimana saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.

Membuat Function
```
function greeting() {
  return 'Hello world';
};
```
Memanggil Function
```
greeting() { // Call the function name
console.log(greeting()); // Output: 'Hello world'
```

### Parameter dan Argumen
1. Parameter
Parameter adalah variabel yang menyimpan nilai untuk diproses di dalam fungsi.
Contoh parameter:
```
function penambahan (a, b) {
  return a + b;
}
```
2. Argumen
Argumen adalah nilai yang digunakan saat memanggil function. Jumlah argumen harus sama dengan jumlah parameternya. Jika di function penambahan ada 2 parameter nilai saat membuat function, saat memanggil function kita juga gunakan 2 buah nilai argumen.
Contoh argumen:
```
function penambahan(a, b) {
  return a + b;
}
console.log(penambahan(5, 5)) // Output: 10
```

Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.

### Default Parameters
Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function. Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argumen.
```
function greetOnWebsite(name = 'Stranger') {
  return 'Hello ' + name;
}
console.log(greetOnWebsite('David')); // Output: 'Hello David'
console.log(greetOnWebsite()); // Output: 'Hello Stranger'
```

### Function Helper
Function helper yaitu kita bisa menggunakan function yang sudah dibuat pada function lain.
```
function multiplyByNineFifths(number) {
  return number * (9/5);
};

function getFahrenheit(celsius) {
  return multiplyByNineFifths(celsius) + 32;
};

getFahrenheit(15); // Returns 59
```

### Arrow Function
Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)
```
const greeting = () => {
  return 'Hello World';
};

const penambahan = (a, b) => {
  return a + b;
};
```

## Data Type Built in Prototype & Method
* Data Type
* String
* Number
* Math
* Primitive & Non Primitive

## DOM
DOM merupakan kependekan dari Document Object Model yang bisa digunakan untuk memanipulasi halaman web HTML agar tampilan website lebih interaktif dan dinamis.

* Mencari Elemen HTML
1. Mengambil elemen dengan ID dengan ``` document.getElementById ```
2. Mengambil Elemen dengan Class dengan ``` document.getElementByClassName ```
3. Mengambil Elemen dengan Nama Tag dengan ``` document.getElementByTagName ```
4. Mengambil Elemen dengan querySelector ``` document.querySelector ```
5. Mengambil Elemen dengan querySelectorAll ``` document.querySelectorAll ```

* Mengubah Konten Element HTML
1. ``` Element.textContent ``` dapat digunakan untuk mengubah teks di dalam sebuah statement.
2. ``` Element.innerHTML ``` dapat digunakan untuk mengubah konten HTML di dalam sebuah statement.

* Membuat Elemen HTML
```
const heading = document.createElement("h1")
heading.textContent = "Ini Heading"

document.getElemntByID("header").appendChild(heading)
```

* HTML DOM Events
1. Click
2. Scroll
3. Change
4. Focus
5. Hover
6. Submit
7. Blur

* Menangkap Interaksi User
1. Element.addEventListener("event)
2. Element.onevent