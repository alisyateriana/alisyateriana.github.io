---
layout: post
title: "Bootstrap"
date: 2025-06-02
---

Materi tentang Bootstrap

## Apa Itu Bootstrap?

Bootstrap adalah framework front-end berbasis HTML, CSS, dan JavaScript 

yang digunakan untuk membangun antarmuka web (UI) yang modern, responsif, 

dan mobile-friendly,Bootstrap dibuat oleh tim dari Twitter pada tahun 2011

(oleh Mark Otto & Jacob Thornton) sebagai solusi agar tampilan web menjadi
 
seragam di berbagai browser dan perangkat. Kini, Bootstrap sudah menjadi

salah satu framework paling populer di dunia pengembangan web.

Tujuan utama Bootstrap adalah membuat desain web lebih cepat, mudah, dan konsisten.

**Kelebihan Bootstrap**

Berikut adalah alasan kenapa Bootstrap banyak digunakan

**Keunggulan	Penjelasan**

Mobile-First	Bootstrap dirancang untuk tampilan perangkat kecil dulu, lalu diperluas.

Responsif	Gunakan grid 12-kolom untuk tampilan fleksibel di semua ukuran layar.

Cepat & Praktis	Tinggal pakai class tanpa menulis CSS panjang.

Komponen Lengkap	Tombol, kartu, form, navigasi, alert, carousel, modal, dll.

Konsisten	Tampilannya stabil di berbagai browser & perangkat.

Dokumentasi	Panduan resmi Bootstrap sangat lengkap dan mudah diikuti.

## Cara Menggunakan Bootstrap

**1. Melalui CDN (Cara Praktis)**

Cukup tambahkan dua baris kode ke dalam file HTML:


<!-- Tambahkan di dalam <head> -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Tambahkan sebelum </body> -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>


**2. Menggunakan NPM (Untuk Proyek Build Tools)**

Jalankan perintah:

npm install bootstrap

Lalu import di file JS atau SCSS kamu:

js
import 'bootstrap/dist/css/bootstrap.min.css';

import 'bootstrap/dist/js/bootstrap.bundle.min.js';

## Komponen-Komponen Penting di Bootstrap

Bootstrap menyediakan banyak komponen siap pakai. Berikut beberapa yang paling sering digunakan:

Tombol

<button class="btn btn-primary">Simpan</button>
<button class="btn btn-danger">Hapus</button>

**1. Navigasi (Navbar)**

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <a class="navbar-brand" href="#">MyWebsite</a>
</nav>

**2.Kartu (Card)**


<div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">Judul Card</h5>
    <p class="card-text">Deskripsi singkat isi konten.</p>
  </div>
</div>

**3. Formulir (Form)**

<form>
  <div class="mb-3">
    <label for="nama" class="form-label">Nama</label>
    <input type="text" class="form-control" id="nama" placeholder="Masukkan nama">
  </div>
</form>

**4 .Peringatan (Alert)**

<div class="alert alert-warning" role="alert">
  Peringatan: Form belum lengkap!
</div>

**5. Modal (Dialog Pop-up)**

<!-- Tombol pembuka -->
<button class="btn btn-success" data-bs-toggle="modal" data-bs-target="#contohModal">Buka Info</button>

<!-- Struktur Modal -->
<div class="modal fade" id="contohModal" tabindex="-1">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title">Judul Modal</h5>
        <button class="btn-close" data-bs-dismiss="modal"></button>
      </div>
      <div class="modal-body">
        Ini isi dari modal popup.
      </div>
    </div>
  </div>
</div>

**6.Sistem Grid di Bootstrap**

Bootstrap menggunakan sistem grid 12 kolom yang fleksibel. Contoh layout 3 kolom seimbang:


<div class="row">
  <div class="col-4">Kolom 1</div>
  <div class="col-4">Kolom 2</div>
  <div class="col-4">Kolom 3</div>
</div>

Grid ini bisa diatur supaya berbeda di layar kecil (mobile) dan besar (desktop), contoh:


<div class="row">

  <div class="col-12 col-md-6">Kolom 1</div>

  <div class="col-12 col-md-6">Kolom 2</div>

</div>

**Kesimpulan**

Bootstrap adalah solusi praktis dan cepat untuk membangun tampilan website yang modern,

responsif, dan user-friendly. Tanpa harus menulis CSS dari awal, kamu bisa menggunakan

berbagai komponen siap pakai hanya dengan menambahkan class tertentu.
