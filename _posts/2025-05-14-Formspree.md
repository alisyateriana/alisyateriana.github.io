---
layout: post
title: "Formspree"
date: 2025-06-23
---

Materi tentang Formspree

## Apa Itu Formspree?

Formspree adalah layanan berbasis cloud yang memungkinkan kamu menerima data

dari formulir HTML langsung ke email tanpa harus membuat backend sendiri,

Dengan kata lain, kamu hanya tinggal membuat form seperti biasa di HTML, 

lalu kirim data pengguna ke Formspree, dan mereka akan meneruskan isinya

ke email milikmu.

Cocok untuk situs statis seperti yang dibuat dengan HTML, GitHub Pages,

Netlify, Vercel, atau bahkan Jekyll!

## Kenapa Pakai Formspree?

Karena tidak semua proyek web membutuhkan backend lengkap. Formspree menjadi 

solusi cepat dan sederhana untuk:

**Website portofolio atau landing page**

Blog pribadi

Proyek tanpa server

Pengembang yang ingin fokus ke frontend

**Cara Kerja Formspree**

Cara kerja Formspree bisa dijelaskan dalam 3 langkah:

Buat form HTML biasa.

Ganti atribut action ke endpoint Formspree (misalnya https://formspree.io/f/abcxyz).

Ketika form dikirim, Formspree akan memproses data lalu mengirimnya ke email kamu.

Tidak perlu PHP, tidak perlu API khusus, semuanya terjadi di sisi Formspree.

**Contoh Form Paling Dasar**

html

<form action="https://formspree.io/f/abcxyz" method="POST">

  <input type="text" name="name" placeholder="Nama" required>

  <input type="email" name="email" placeholder="Email" required>


  <textarea name="message" placeholder="Pesan..." required></textarea>

  <button type="submit">Kirim</button>

</form>

Gantilah https://formspree.io/f/abcxyz dengan endpoint milikmu sendiri 
yang bisa kamu dapatkan setelah mendaftar di situs Formspree.

Fitur-Fitur Keren Formspree

Kirim Langsung ke Email

Setiap kali form dikirim, kamu langsung dapat notifikasi email berisi data isian dari pengguna.

**edirect Setelah Submit**

Kamu bisa mengarahkan user ke halaman "Terima Kasih" menggunakan:

html

<input type="hidden" name="_redirect" value="https://websitekamu.com/thanks.html">

**Proteksi Anti-Spam**

Gunakan honeypot (field tersembunyi) untuk menangkal bot

Dukung Google reCAPTCHA (di versi Pro)

**Validasi**

Gunakan validasi HTML5 biasa (seperti required, type="email"), dan Formspree

akan menghormati validasi tersebut.

**Custom Email Subject**

Kamu bisa mengatur subjek email:

html

<input type="hidden" name="_subject" value="Pesan Baru dari Website">

**Integrasi API & Webhook**

Kamu bisa hubungkan data dari form ke:

Google Sheets

Zapier

Notifikasi Slack

atau backend kamu sendiri melalui Webhook

**Cara Menggunakan Formspree (Langkah Singkat)**

Daftar akun di formspree.io

Buat project baru dan ambil URL endpoint (contoh: https://formspree.io/f/xyzabc)

Masukkan URL tersebut ke dalam atribut action form HTML

Tambahkan field name, email, message, dsb.

Kirim form, dan data akan masuk ke email kamu

(Opsional) Tambahkan redirect, validasi, dan keamanan

**Contoh Form Lengkap + Fitur Tambahan**

html

<form action="https://formspree.io/f/xyzabc" method="POST">

  <label>Nama:

    <input type="text" name="nama" required>

  </label>

  <label>Email:

    <input type="email" name="_replyto" required>

  </label>

  <label>Topik:

    <select name="topik">

      <option value="dukungan">Dukungan</option>

      <option value="saran">Saran</option>

    </select>

  </label>

  <label>Pesan:

    <textarea name="pesan" required></textarea>

  </label>

  <!-- Redirect, subject, reply -->
  <input type="hidden" name="_subject" value="Pesan Baru dari Form!">
  <input type="hidden" name="_redirect" value="https://websitekamu.com/terima-kasih.html">

  <!-- Anti-Spam (honeypot) -->
  <input type="text" name="_gotcha" style="display:none">

  <button type="submit">Kirim</button>
</form>

**Tips Praktis**

Selalu pakai atribut required untuk validasi

Tambahkan _replyto agar bisa langsung membalas dari email

Gunakan honeypot agar form tidak mudah dimanfaatkan bot

Siapkan halaman thank-you.html untuk pengalaman pengguna yang baik

Untuk kebutuhan kompleks, upgrade ke Formspree Pro agar bisa pakai reCAPTCHA dan webhook

Dokumentasi & Bantuan

Website resmi Formspree

Dokumentasi lengkap

GitHub Repository

**Kesimpulan**

Formspree adalah solusi praktis untuk menerima input dari pengguna tanpa 

backend rumit, Cukup buat form HTML biasa, hubungkan ke endpoint Formspree,

dan biarkan mereka mengurus sisanya—mulai dari validasi hingga pengiriman email.

Dengan fitur seperti notifikasi email, integrasi API, proteksi spam, dan kemudahan 

penggunaan, Formspree sangat ideal untuk pengembang front-end dan website statis.