# WRITING TEST - WEEK 3
## Array
Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya. Array dapat menyimpan tipe data String, Number, Boolean, dan lainnya.

Contoh Array:
```
let productTeam = ['Product Manager', 'Front End Developer', 'Back End Developer'];
console.log(productTeam);
```

### Membuat Array
* Array didefinisikan menggunakan square brackets []

### Mengakses/Memanggil Array
* Array pada javascript dihitung dari index data ke-0.
* Data pertama adalah index ke-0.
```
let todoList = [
    'Belajar javascript',
    'Mencuci baju',
    'Latihan membuat aplikasi javascript'
    ];
console.log(todoList[0]); //Output : Belajar javascript
console.log(todoList[2]); //Output : Latihan membuat aplikasi javascript
```

### Update Array
Seperti tipe data dan variabel pada umumnya, kita dapat mengupdate data pada Array
```
let productTeam = ['Product Manager', 'Front End Developer', 'Back End Developer'];
productTeam[0] = 'Product Designer';
console.log(productTeam);
//Output : ['Product Manager', 'Front End Developer', 'Back End Developer', 'Product Designer'];
```

### Const in Array
* Jika menggunakan let, kita dapat mengubah array  dengan array baru dan konten nilai yang ada di dalam array dengan nilai lain
* Const tidak bisa melakukan update data. Namun pada Array kita dapat melakukan update konten nilai di dalam array (mutable).
* Yang tidak bisa adalah mengubah array dengan array yang baru jika menggunakan const

const cars = ['tesla', 'honda', 'toyota'];
cars[2] = ['nissan'];
console.log(cars);
// Output: ['tesla', 'honda', 'toyota']

### Array Properties
Properties adalah fitur yang sudah disediakan oleh Javascript untuk memudahkan developer. Array memiliki 5 properti yang sering digunakan yaitu constructor, length, index, input, dan prototype.

* ```.length```
length akan mengembalikan nilai dari jumlah panjang data suatu array.

let productTeam = ['Product Manager', 'Front End Developer', 'Back End Developer'];
console.log(productTeam.length);
//Output: 3

### Array Method
Array memiliki method atau biasa disebut built-in methods. Artinya Javascript sudah memudahkan kita dengan menyediakan function/method umum yang bisa kita gunakan.
* ```.push()``` adalah method untuk menambahkan item  array pada urutan yang paling akhir.
* ```.pop()``` adalah method yang menghapus item array index terakhir.
* ```.shift()``` adalah method untuk menghapus item Array pada index pertama
* ```.sort()``` adalah method untuk mengurutkan secara Ascending atau Descending Alphanumeric

### Looping pada Array
* ```.forEach()``` adalah method untuk melakukan looping pada setiap elemen array.
* ```.map()``` melakukan perulangan/looping dengan membuat array baru.

```.map()``` dan ```.forEach()``` sama-sama melakukan looping dan mengembalikan nilai baru dari operasi yang dilakukan. Perbedaannya adalah ```.forEach()``` tidak dapat membuat Array baru dari hasil operasi yang ada dalam looping

## Multidimensional Array
Multidimensional Array bisa dianalogikan dengan array of array (ada array didalam array).

Akses Multidimensional Array:
```
let inventory = {
    ['Kaos Polos', 10],
    ['Jaket Hoodie', 12],
    ['Topi', 24],
    ['Celana Jeans', 8],
};
console.log(inventory[1][0]);
//Output: Jaket Hoodie
```

## Object
Object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method).
* Properti adalah data lengkap dari sebuah object.
* Method adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.

### Membuat sebuah object
```
let person = {
    name = 'John Doe',
    age: 25,
    isVerified: true,
}
```

### Mengakses Object dan Property Object
```
let person = {
    name = 'John Doe',
    age: 25,
    isVerified: true,
}

//Call variable with the property
console.log(person.name); //John Doe
```

### Update Object
```
let person = {
    name = 'John Doe',
    age: 25,
    isVerified: true,
}

//update key yang sudah ada dengan value yang baru
person.age = 27;

//menambah key dan value baru
person.address = "London, UK";

console.log(person);
```

### Delete Object
```
let person = {
    name = 'John Doe',
    age: 25,
    isVerified: true,
}

delete person.age;

console.log(person);
```

## Recursive
Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu. Recursive kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.

Contoh rekursif
```
function pow(x,n) {
    if (n ==1) {
        return x;
        }
        else {
            return x * pow(x, n -1);
        }
    }
}

console.log(pow(2,3)); //8
```

Recursive akan berhenti memanggil dirinya sendiri jika kondisi terpenuhi.

