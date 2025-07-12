---
layout: post
title: "Single Menu"
date: 2025-06-23
---

Materi tentang Single Menu


## Penjelasan Lengkap tentang Single Menu dalam UI dan Form

Secara umum, Single Menu dalam dunia UI (User Interface) merujuk pada komponen

pemilihan (selection input) yang hanya memperbolehkan satu pilihan aktif dalam 

satu waktu. Komponen ini banyak digunakan dalam formulir, pengaturan sistem,

survei online, maupun tampilan antarmuka aplikasi berbasis web dan mobile.

Single Menu berbeda dengan navigasi menu utama (seperti menu Home, About, 

Contact), karena fokusnya bukan pada navigasi antar halaman, melainkan pada

 pilihan antar opsi dalam satu konteks.

## Tujuan Penggunaan

Single Menu dirancang untuk Menyederhanakan pilihan bagi pengguna

Menghindari ambiguitas input (karena hanya satu pilihan yang diizinkan)

Mengarahkan pengguna untuk mengambil keputusan dengan cepat Meningkatkan 

pengalaman pengguna (user experience) melalui antarmuka yang efisien dan rapi

## Jenis-Jenis Komponen Single Menu

Berikut adalah jenis-jenis komponen pilihan tunggal dan ganda (single & multiple choice),

dengan fokus utama pada Single Menu (single choice):

## 1. Radio Button – Komponen Pilihan Tunggal Klasik

Fungsi Utama Memungkinkan pengguna memilih satu saja dari sekumpulan pilihan yang tersedia.

Contoh HTML

<p>Pilih status:</p>
<input type="radio" name="status" value="aktif"> Aktif<br>
<input type="radio" name="status" value="nonaktif"> Nonaktif<br>
<input type="radio" name="status" value="pending"> Pending

Karakteristik Semua input radio harus memiliki atribut name yang sama agar sistem mengenal

bahwa mereka dalam satu grup. Saat salah satu dipilih, yang lain otomatis tidak aktif,

Cocok digunakan untuk data seperti Jenis kelamin Status akun Kategori pilihan tetap 

(misalnya, metode pengiriman)

## Kelebihan

Mudah dipahami oleh pengguna

Tidak membutuhkan JavaScript

Kompatibel di semua browser

## Kekurangan

Jika terlalu banyak pilihan, antarmuka menjadi panjang

## 2. Toggle Button / Button Group – Versi Interaktif dari Radio Button

Fungsi Utama Memberikan pengalaman pemilihan satu dari beberapa opsi, namun 

dalam bentuk tombol yang lebih interaktif dan estetik.

Contoh HTML (Bootstrap 5)


<div class="btn-group" role="group">
  <input type="radio" class="btn-check" name="viewmode" id="grid" autocomplete="off" checked>
  <label class="btn btn-outline-primary" for="grid">Grid</label>

  <input type="radio" class="btn-check" name="viewmode" id="list" autocomplete="off">
  <label class="btn btn-outline-primary" for="list">List</label>
</div>

## Karakteristik

Menggunakan input type="radio" namun disajikan sebagai tombol

Sering digunakan dalam aplikasi modern (terutama mobile)

Memberikan feedback visual saat tombol aktif

## Kelebihan

Tampil modern dan interaktif

Mudah dipadukan dengan framework UI seperti Bootstrap

Cocok untuk pengaturan visual, mode tampilan, dll.

## Kekurangan

Membutuhkan CSS tambahan atau library seperti Bootstrap

Bisa membingungkan jika tidak diberi label yang jelas

## 3. Checkbox – Pilihan Ganda (Bukan Single Menu, tapi Penting Diketahui)

Fungsi Utama Digunakan ketika pengguna boleh memilih lebih dari satu opsi.

Contoh HTML

<p>Pilih minat:</p>
<input type="checkbox" name="minat[]" value="musik"> Musik<br>
<input type="checkbox" name="minat[]" value="membaca"> Membaca<br>
<input type="checkbox" name="minat[]" value="game"> Bermain Game

## Karakteristik

Checkbox tidak saling eksklusif

Cocok untuk

Minat atau hobi

Fitur tambahan

Multi-tag atau multi-kategori

Note: Checkbox termasuk kategori multiple choice dan bukan bagian dari single menu, tapi perlu diketahui karena penggunaannya sangat dekat.

## 4. Select / Combo Box – Dropdown Menu

Fungsi Utama

Menampilkan daftar pilihan dalam bentuk dropdown agar hanya satu opsi yang bisa dipilih (default).

Contoh HTML:

<label for="jurusan">Pilih jurusan:</label>
<select id="jurusan" name="jurusan">
  <option value="tkj">TKJ</option>
  <option value="rpl">RPL</option>
  <option value="mm">Multimedia</option>
</select>

## Karakteristik

Secara default hanya bisa memilih satu

Untuk multi-select, tambahkan atribut multiple

Cocok digunakan untuk:

Provinsi/Kota

Negara

Kategori produk

Pilihan yang panjang

## Kelebihan

Hemat tempat di UI

Praktis untuk pilihan yang panjang

Mudah diimplementasikan

## Kekurangan

Tidak menampilkan semua pilihan secara langsung

Kurang intuitif untuk pengguna baru jika opsi terlalu banyak

