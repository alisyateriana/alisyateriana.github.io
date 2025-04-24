---
layout: post
title: "Instalasi Ruby dan Jekyll"
date: 2025-02-20
---

Materi tentang Instalasi Ruby dan Jekyll


# Instalasi Ruby dan Jekyll 🛠️

Untuk memulai membuat blog menggunakan Jekyll, pastikan kamu sudah menginstal Ruby dan Jekyll di komputer kamu. Jekyll adalah sebuah static site generator yang memungkinkan kamu membuat blog atau website tanpa perlu menggunakan database.

## Langkah 1: Instalasi Ruby 📦
- **Windows**: Kamu bisa mengunduh Ruby menggunakan [RubyInstaller](https://rubyinstaller.org/). Ikuti petunjuk untuk menginstal Ruby di komputer kamu.
- **macOS/Linux**: Kamu bisa menginstal Ruby dengan menggunakan Homebrew di macOS atau menggunakan package manager di Linux. Jalankan perintah berikut di terminal:
  ```bash
  brew install ruby
  ```

## Langkah 2: Instalasi Jekyll 🚀
Setelah Ruby terinstal, langkah selanjutnya adalah menginstal Jekyll. Untuk menginstalnya, buka terminal dan jalankan perintah berikut:
```bash
gem install jekyll bundler
```
Perintah ini akan menginstal Jekyll dan Bundler, yang berguna untuk mengelola dependensi dalam proyek Jekyll kamu.

## Langkah 3: Membuat Proyek Jekyll Baru 💻
Setelah instalasi selesai, kamu bisa membuat proyek baru dengan perintah berikut:
```bash
jekyll new nama-proyek
cd nama-proyek
jekyll serve
```
Proyek baru kamu sekarang sudah bisa diakses di `http://localhost:4000` di browser. Jika berhasil, kamu akan melihat halaman depan website Jekyll yang sudah siap digunakan.

## Masalah Umum:
- **Jika mendapat error**: Pastikan Ruby dan Jekyll sudah terinstal dengan benar. Jika perlu, coba update Ruby atau periksa kompatibilitas versi.
- **Solusi jika error**: Jika masalah berlanjut, kamu bisa mencari bantuan di [forum Jekyll](https://talk.jekyllrb.com/).
