---
layout: post
title: "Layout dan Navigasi"
date: 2025-03-13
---

Materi tentang Layout dan Navigasi

# Layout dan Navigasi 🖥️

Layout di Jekyll digunakan untuk membuat struktur halaman yang konsisten di seluruh situs. Layout ini memungkinkan kamu mengatur header, footer, dan elemen lainnya di seluruh halaman blog kamu.

## Menyiapkan Layout:

1. **File `_layouts/default.html`** adalah template dasar yang akan digunakan oleh halaman lain. Berikut adalah contoh layout untuk halaman utama dengan navigasi:

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="UTF-8" />
       <meta name="viewport" content="width=device-width, initial-scale=1.0" />
       <title>{{ page.title }}</title>
     </head>
     <body>
       <header>
         <nav>
           <ul>
             <li><a href="/">Home</a></li>
             <li><a href="/about">About</a></li>
             <li><a href="/blog">Blog</a></li>
           </ul>
         </nav>
       </header>

       <main>{{ content }}</main>

       <footer>
         <p>&copy; 2025 Balqis Misyia</p>
       </footer>
     </body>
   </html>
   ```

2. **Navigasi**:
   Navigasi adalah bagian penting dari setiap website. Di atas, kita sudah membuat navigasi dasar menggunakan `<ul>` untuk daftar tautan.

## Menambahkan Halaman:

- **About Page**: Buat halaman `about.md` dengan konten tentang kamu, dan Jekyll akan otomatis menghubungkannya dengan navigasi.

## Tips:

- Jangan lupa untuk menambahkan CSS di file `assets/css/style.css` agar tampilan lebih menarik.
- Gunakan **partials** untuk elemen yang sering muncul seperti header dan footer, supaya kamu tidak perlu menulis kode yang sama berulang-ulang.
