---
layout: post
title: "HTML: Link dan List"
date: 2025-03-20
---

Materi tentang link dan lists pada HTML

# Link dan List dalam HTML 🔗

HTML adalah bahasa dasar yang digunakan untuk membuat website, dan di dalamnya terdapat elemen-elemen seperti **link** dan **list** yang sangat berguna.

## Tautan (Link) 🖇️:

Tautan digunakan untuk menghubungkan halaman-halaman di dalam website atau bahkan ke situs luar. Berikut cara membuat tautan di HTML:

```html
<a href="https://www.google.com" target="_blank">Klik di sini untuk Google</a>
```

- **`target="_blank"`** akan membuka tautan di tab baru.

## Daftar (List) 📜:

HTML juga memungkinkan kamu untuk membuat daftar, baik berurutan maupun tidak berurutan.

- **Daftar Tidak Berurutan** (bullets):

  ```html
  <ul>
    <li>Item pertama</li>
    <li>Item kedua</li>
    <li>Item ketiga</li>
  </ul>
  ```

- **Daftar Berurutan** (nomor):
  ```html
  <ol>
    <li>Langkah pertama</li>
    <li>Langkah kedua</li>
    <li>Langkah ketiga</li>
  </ol>
  ```

## Menambahkan Tautan ke Daftar:

Kamu bisa juga menambahkan tautan di dalam daftar untuk membuat menu atau daftar isi.

```html
<ul>
  <li><a href="#section1">Bagian 1</a></li>
  <li><a href="#section2">Bagian 2</a></li>
  <li><a href="#section3">Bagian 3</a></li>
</ul>
```
