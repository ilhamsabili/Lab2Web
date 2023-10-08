# Lab2Web
Nama : Ilham Sabili

NIM  : 312210120

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksipraktikum)|
|2|Praktikum|[Click Here](#praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaandantugas)|

## Instruksi Praktikum 
> 1. Persiapkan text editor misalnya VSCode.
> 2. Buat file baru dengan nama `lab2_css_dasar.html`
> 3. Buat struktur dasar dari dokumen HTML.
> 4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
> 5. Lakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/


## Praktikum 
### 1. Membuat dokumen HTML
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Dasar</title>
  </head>
  <body>
    <header>
      <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
      <a href="lab2_css_dasar.html">CSS Dasar</a>
      <a href="lab2_css_eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p>
        Kami sedang belajar HTML dan CSS dasar, pada mata kuliah
        <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran
        pertama yang kami dapat adalah membuat tampilan web sederhana dalam
        rangka mengenal tag-tag dasar HTML dan CSS.
      </p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
    </div>
  </body>
</html>
```
> - Maka hasilnya akan seperti berikut : 

![1,1](https://github.com/ilhamsabili/Lab2Web/assets/115677697/8a3f6432-dffd-4c0e-8edb-084fd227d0a9)




### 2. Mendeklerasikan CSS Internal
```
<head>
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>
```
> - Maka hasilnya akan seperti berikut :

![2](https://github.com/ilhamsabili/Lab2Web/assets/115677697/91bf85b7-fe28-44f3-bcdf-565e1d5ec403)



> - CSS internal adalah css yang filenya di letakan dalam html dengan pendeklarasian style.


### 3. Menambahkan Inline CSS
> - Menambahkan Inline CSS, kemudian tambahkan deklarasi inline CSS pada tag `<p>`
```
<p style="text-align: center; color: #ccd8e4;">
```
> - Maka hasilnya akan seperti berikut :

![3](https://github.com/ilhamsabili/Lab2Web/assets/115677697/592d61ff-e213-4bd8-ab7b-8863b2b2a776)




### 4. Membuat CSS Eksternal
> - Membuat CSS Eksternal dengan membuat file baru dengan nama **style_eksternal.css** kemudian buat deklarasi css seperti berikut ini.
```
nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}
```
> - Kemudian tambahkan <link untuk merujuk File CSS yang telah dibuat pada bagian `<head>`
```
<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```

> - Maka hasilnya akan seperti berikut :

![4](https://github.com/ilhamsabili/Lab2Web/assets/115677697/1f555e5e-1dd9-420a-b467-3e378d577815)



> - CSS ekternal adalah CSS yang file di tempatkan di luar file HTML dengan menambahkan link dalam HTML agar tertaut dengan file CSS

### 5. Menambahkan CSS Selector
> - Selanjutnya menambahkan CSS Selector menggunkan ID dan class Selector pada file **style_eksternal.css** dan menambahkan kode seperti berikut :
```
/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}
```
> - Maka hasilnya akan seperti berikut :

![5](https://github.com/ilhamsabili/Lab2Web/assets/115677697/cad14eed-2cc8-4def-9502-28cae07beb40)



> - CSS Selector terdiri atas selector ID, Selector Class, Dan Selector elemen Selector ID pendeklarasiannya yaitu dengan (#), Sedangkan Class pendeklarasiannya yaitu dengan (.), Dan Selector elemen pendeklarasiannya dengan elemen HTML sebagai contoh (p) yang akan di beri gaya pada CSS.

### 6. MeLakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/

![Screenshot (24)](https://github.com/syifaaurellia/Lab2web/assets/115867244/b83d42a1-b3fd-4f97-bf22-e394ae012158)


![Screenshot (25)](https://github.com/syifaaurellia/Lab2web/assets/115867244/f878a92d-b2f3-40cb-81d9-bb682245c62b)

## Pertanyaan dan Tugas 

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
> Jawaban :

![j1](https://github.com/ilhamsabili/Lab2Web/assets/115677697/878235ea-b951-43f9-b974-31c8021fa796)



![j2](https://github.com/ilhamsabili/Lab2Web/assets/115677697/b2176a09-6384-44c7-8a12-0a0f4c5af19d)



- Pada contoh ini, terdapat elemen `<h1> dengan class "title"` dan `elemen <p> dengan class "text"`. Class tersebut akan digunakan sebagai selector dalam CSS untuk mengubah properti dan nilai. Dalam file CSS (style.css), terdapat aturan CSS yang dideklarasikan untuk `class "title" dan "text"`. Aturan tersebut mengubah properti `"color"` pada elemen dengan class tersebut. Anda dapat mengubah nilai properti `"color"` pada file CSS sesuai keinginan Anda untuk melihat perubahan yang terjadi pada `judul (h1)` dan `paragraf (p)` dalam hal warna teks.


2. Apa perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}?` berikan penjelasannya!
> Jawaban :

- `h1 {...}` : Deklarasi ini akan merubah semua elemen "h1".

- `#intro h1 {...}` : Deklarasi ini lebih spesifik, maksud nya adalah pendeklarasian yang mengacu kepada pemberian atribut pada elemen "h1" dengan menambahkan id "intro".


3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
> Jawaban :

- Ketika kita mendeklarasikan secara bersamaan antara **INTERNAL EKSTERNAL** dan **INLINE** yang akan ditampilkan pada Browser adalah **INLINE**, karena **INLINE** memiliki prioritas dibanding **EKSTERNAL** atau pun **INTERNAL** seperti contoh yang saya buat, saya membuat dokumen baru HTML kemudian saya buat Elemen `{h1}`yang kemudian saya akan deklarasikan di CSS **INTERNAL EKSTERNAL** dan juga **INLINE** Dengan property `{color}` dengan warna yang berbeda,jika **INTERNAL** `{color: red}` sementara **EKSTERNAL** `{color:blue;}` dan **INLINE** `{color: green;}` yang terpanggil dibrowser adalah **INLINE** karena memiliki prioritas.


![j3](https://github.com/ilhamsabili/Lab2Web/assets/115677697/baac4059-6a8e-4c2a-bfc9-3074592c3049)



- Pict di atas adalah deklarasi **INLINE** dan **INTERNAL**, sementara pict di bawah adalah deklarasi **EKSTERNAL**.


![j4](https://github.com/ilhamsabili/Lab2Web/assets/115677697/162766d7-94b0-4343-ab77-e82bb1e6a094)



- Jadi yang terpanggil adalah **CSS INLINE** karena memiliki prioritas tinggi dibanding CSS deklarasi lainnya.


4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
> Jawaban :

```
( <p id="paragraf-1" class="text-paragraf"> )
```
- Yang terpanggil di browser adalah **ID** karena **ID** bersifat unik berbeda dengan **Class**. **Class** bisa digunakan banyak sementara **ID** hanya tertentu saja itu kenapa **ID** unik dan yang terpanggil di browser adalah **ID**.


![j5](https://github.com/ilhamsabili/Lab2Web/assets/115677697/f9227953-47f3-4069-99a8-09822ee851f5)



- Di atas saya menambahkan property `{color}` dan `{text-align}` untuk **ID {color: orchid}** dan **{text-align: center}** sementara Class yaitu **{color:palegreen}** dan **{text-align: left}**. Namun yang terpanggil di browser adalah **ID** yang property nya **{color: orchid}** dan juga **{text-align: center}**



## Finish, Terima Kasih 
