---
layout: post
title: "SASS dan SCSS"
date: 2025-05-07
---

Materi tentang SASS dan SCSS


## Apa Itu SASS dan SCSS?

SASS dan SCSS adalah bagian dari Sass (Syntactically Awesome Stylesheets), 

yaitu CSS Preprocessor yang memungkinkan kamu menulis CSS dengan fitur yang

lebih canggih dan efisien.

Sass membuat CSS lebih powerful, modular, dan lebih mudah dikelola dalam proyek besar.

**1. Apa Itu SASS?**

SASS adalah format lama (indented syntax) dari Sass yang tidak menggunakan tanda kurung

{} dan titik koma ;, melainkan menggunakan indentasi (spasi/tab) sebagai penanda blok.

**Contoh SASS (Indent-Based Syntax)**

sass
$primary-color: #e67e22

body
  background-color: $primary-color

h1
  font-size: 2rem
  color: white
🔧 Karakteristik SASS:
Tidak menggunakan {} atau ;

Penulisan lebih ringkas

Cocok bagi yang menyukai gaya minimalis seperti Python

**2. Apa Itu SCSS?**

SCSS (Sassy CSS) adalah versi modern dari Sass yang menggunakan sintaks mirip 

CSS biasa — lengkap dengan kurung kurawal {}, titik koma ;, dan aturan CSS standar.

**Contoh SCSS (CSS-like Syntax)**

scss
$primary-color: #e67e22;

body {
  background-color: $primary-color;
}

h1 {
  font-size: 2rem;
  color: white;
}

**Karakteristik SCSS**

Semua file CSS valid juga merupakan file SCSS valid

Lebih mudah diadopsi oleh developer yang sudah terbiasa dengan CSS

Saat ini lebih populer dan sering digunakan

## Fitur Unggulan SASS/SCSS (yang tidak ada di CSS biasa)

Fitur	Fungsi

Variabel	Menyimpan nilai warna, font, ukuran, dll.

Nesting	Menulis selector CSS di dalam selector lain (mirip struktur HTML)

Partials	Membagi file CSS besar ke file kecil dan mengimpor kembali (@use)

Mixin	Blok kode CSS reusable dengan parameter

Inheritance (@extend)	Mewarisi style dari selector lain

Function	Membuat fungsi kustom untuk logika styling

Contoh Fitur SCSS

**Variabel**

scss
$main-font: 'Poppins', sans-serif;
$bg-color: #f4f4f4;

body {
  font-family: $main-font;
  background-color: $bg-color;
}

**Nesting**

scss
nav {
  ul {
    list-style: none;
    li {
      display: inline-block;
      a {
        text-decoration: none;
        color: blue;
      }
    }
  }
}

**Mixin**

scss
@mixin card($radius) {
  padding: 1rem;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  border-radius: $radius;
}

.card {
  @include card(12px);
}
🔹 Extend (Inheritance)
scss
%base-button {
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}

.btn-primary {
  @extend %base-button;
  background-color: blue;
  color: white;
}

.btn-secondary {
  @extend %base-button;
  background-color: gray;
}

## Perbedaan SASS vs SCSS

Fitur	SASS	SCSS

Sintaks	Indentasi (tanpa {} dan ;)	Seperti CSS (pakai {} dan ;)

Populeritas	Kurang populer, digunakan khusus	Lebih umum, banyak digunakan

Kemudahan	Lebih singkat, tapi harus hati-hati indentasi	Lebih fleksibel, cocok untuk semua

## Kesimpulan

SASS dan SCSS adalah alat bantu untuk menulis CSS dengan cara yang lebih terstruktur, 

efisien, dan canggih.

SCSS lebih umum digunakan karena kompatibel dengan CSS.

Dengan menggunakan SCSS/SASS, kamu dapat:

Menyederhanakan file CSS besar

Menggunakan variabel dan fungsi

Membuat styling lebih modular dan reusable

Jadi, untuk proyek front-end modern, SCSS/SASS sangat direkomendasikan agar

kodenya tidak hanya cantik di tampilan, tapi juga rapi dan mudah dikelola di balik layar. 

Kalau kamu ingin, aku bisa bantu buatkan template folder SCSS lengkap dengan main.scss,

partials seperti _variables.scss, _mixins.scss, dan cara kompilasinya ke CSS menggunakan

Sass CLI atau Live Sass Compiler di VS Code. Cukup bilang saja!














