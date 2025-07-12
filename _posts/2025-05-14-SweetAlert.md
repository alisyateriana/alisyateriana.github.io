---
layout: post
title: "SweetAlert"
date: 2025-05-12
---

Materi tentang SweetAler

## Apa itu SweetAlert?

SweetAlert adalah pustaka JavaScript yang digunakan untuk menampilkan popup 

alert (kotak dialog peringatan) dengan tampilan yang lebih menarik dan

interaktif dibandingkan alert bawaan browser (window.alert()).

## Fungsi Utama SweetAlert

SweetAlert digunakan dalam banyak skenario di pengembangan web, seperti:

Menampilkan pesan sukses (success message)

Memberi peringatan atau konfirmasi sebelum aksi penting

Memberi tahu error atau kesalahan

Meminta input dari pengguna (hanya di versi SweetAlert2)

Meningkatkan user experience dengan tampilan popup yang keren

Dua Versi: SweetAlert vs SweetAlert2

Aspek	SweetAlert (v1)	SweetAlert2 (v2)

Tampilan	Sederhana & statis	Modern, responsif, halus

Form input	Tidak didukung	 Mendukung berbagai input

Kustomisasi tombol	Terbatas	Lebih lengkap & fleksibel

Dokumentasi	Kurang aktif	Selalu update & lengkap

Dukungan animasi	Dasar	 Lebih smooth dan menarik

## Rekomendasi: Gunakan SweetAlert2 karena lebih fleksibel dan kaya fitur.

**Cara Menggunakan SweetAlert**

**1. Tambahkan Library**

Menggunakan CDN (untuk HTML biasa):


<!-- SweetAlert2 -->
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>

**2.Menggunakan NPM (untuk React, Vite, Laravel, dll)**


**npm install sweetalert2**

Contoh Penggunaan

Notifikasi Sukses

js

Swal.fire({

  title: 'Berhasil!',

  text: 'Data sudah disimpan.',

  icon: 'success',

  confirmButtonText: 'OK'

});


**Konfirmasi Aksi**

js

Swal.fire({

  title: 'Hapus data?',

  text: 'Data ini tidak bisa dikembalikan.',

  icon: 'warning',

  showCancelButton: true,

  confirmButtonText: 'Ya, hapus!',

  cancelButtonText: 'Batal',

  confirmButtonColor: '#e3342f',

  cancelButtonColor: '#6c757d'

});


**Auto Close (Timer)**

js

Swal.fire({

  title: 'Loading...',

  text: 'Popup ini akan tertutup otomatis.',

  timer: 3000,

  showConfirmButton: false

});


**Input dari Pengguna**

js

Swal.fire({

  title: 'Masukkan email kamu',

  input: 'email',

  inputPlaceholder: 'email@example.com',

  showCancelButton: true,

  inputValidator: (value) => {

    if (!value) return 'Email tidak boleh kosong!';

  }

});


**Callback Setelah Konfirmasi**

js

Swal.fire({

  title: 'Yakin logout?',

  icon: 'question',

  showCancelButton: true,

  confirmButtonText: 'Ya',

}).then((result) => {

  if (result.isConfirmed) {

    // misalnya redirect atau AJAX

    window.location.href = '/logout';

  }

});

**3.Integrasi SweetAlert2 dengan Framework**

**jQuery**

<button id="btn">Klik Saya</button>
<script>
  $('#btn').on('click', () => {
    Swal.fire('Diklik!', 'Tombol berhasil ditekan.', 'info');
  });
</script>

**React**

js
import Swal from 'sweetalert2';

function handleClick() {
  Swal.fire('Hello React!', 'Ini contoh dari SweetAlert2', 'info');
}

**Laravel Blade**


<a onclick="konfirmasi()">Hapus</a>
<script>
function konfirmasi() {
  Swal.fire({
    title: 'Hapus data?',
    text: 'Tindakan ini tidak bisa dibatalkan!',
    icon: 'warning',
    showCancelButton: true,
    confirmButtonText: 'Ya, hapus!'
  }).then((res) => {
    if (res.isConfirmed) {
      window.location.href = '/hapus';
    }
  });
}
</script>

**Tips Penggunaan**

Gunakan ikon & warna sesuai konteks (merah untuk error, hijau untuk sukses)

Jangan tampilkan popup terlalu sering (bisa mengganggu pengguna)

Gunakan promise chaining (.then()) untuk aksi lanjutan

Selalu test tampilan popup di berbagai browser

**Dokumentasi Resmi**

SweetAlert (v1)

SweetAlert2

**Kesimpulan**

SweetAlert (dan SweetAlert2) adalah alat modern untuk mempercantik notifikasi 

dan konfirmasi dalam aplikasi web. Dengan desain elegan, ikon menarik, dan kemampuan

interaktif seperti input form, SweetAlert membuat website kamu terlihat lebih profesional

dan nyaman digunakan.