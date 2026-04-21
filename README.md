⚡ Sann Store — Test Web

Sann Store adalah sebuah frontend e-commerce mockup berbasis HTML, CSS, dan JavaScript murni (vanilla JS) tanpa framework. Project ini dibuat sebagai simulasi tampilan dan interaksi toko online modern dengan fitur yang cukup lengkap di sisi client.

«⚠️ Catatan: Ini bukan production-ready app. Tidak ada backend, database, atau sistem pembayaran real.»


✨ Fitur Utama

🛍️ Produk & UI

- Grid produk responsif
- Kategori produk (Gadget, Fashion)
- Sorting:
  - Harga termurah
  - Harga termahal
  - Rating tertinggi
- Live search (real-time filtering)

❤️ Wishlist

- Tambah/hapus produk ke wishlist
- Disimpan di "localStorage"
- Counter otomatis di navbar

🛒 Keranjang (Cart)

- Tambah produk ke cart
- Update quantity (+ / -)
- Perhitungan subtotal & total otomatis
- Persist data via "localStorage"

🎟️ Promo Code

- Sistem diskon berbasis persen
- Support max discount limit
- Contoh:
  - "sannganteng"
  - "test"

📦 Checkout

- Generate order summary
- Redirect ke WhatsApp dengan pesan otomatis
- Simpan riwayat pembelian (history)

📜 Riwayat Pembelian

- Menyimpan transaksi di localStorage
- Expandable detail per order

🌙 Theme

- Dark / Light mode toggle

🔥 Flash Sale

- Countdown timer real-time

🔔 UX Enhancement

- Toast notification
- Modal system (cart, wishlist, detail, history)
- Product detail + rekomendasi produk


🧠 Arsitektur

Semua logic dikendalikan oleh satu object utama:

const app = { ... }

State Management (Client-side)

- "cart" → data keranjang
- "wishlist" → produk favorit
- "history" → riwayat order
- "products" → data statis produk
- "activePromo" → promo aktif

Semua state disimpan menggunakan:

localStorage


📂 Struktur Project

.
├── index.html   # Semua (HTML + CSS + JS)

Tidak ada dependency build tools atau package manager.


🚀 Cara Menjalankan

1. Download / clone repo:

git clone https://github.com/username/sann-store.git

2. Buka file:

index.html

3. Jalankan di browser (double click / live server)


⚙️ Konfigurasi

Nomor WhatsApp Checkout

Ubah di bagian ini:

const phoneNumber = '447723442693';


Data Produk

Edit di:

const productsData = [ ... ];


Promo Code

Edit di:

const PROMO_CODES = {
    'sannganteng': { type: 'percent', value: 0.1, max: 9999999 },
    'test': { type: 'percent', value: 0.7, max: 100000 }
};


⚠️ Keterbatasan

- Tidak ada backend (semua fake / mock)
- Tidak ada autentikasi user
- Tidak ada payment gateway
- Tidak scalable untuk production
- Data bisa hilang jika "localStorage" dihapus


🧪 Tujuan Project

Project ini cocok untuk:

- Latihan frontend logic tanpa framework
- Portfolio UI/UX
- Belajar DOM manipulation
- Simulasi e-commerce flow


🧩 Potensi Pengembangan

Jika mau dinaikkan levelnya:

- Integrasi backend (Node.js / Laravel)
- Database (MySQL / MongoDB)
- Authentication system
- Real payment gateway (Midtrans, Stripe, dll)
- State management lebih modular
- Refactor ke React / Vue / Next.js


📜 Lisensi

Bebas digunakan untuk pembelajaran dan pengembangan pribadi.


🧠 Catatan

Project ini menunjukkan satu hal sederhana:

«E-commerce pada dasarnya bukan soal "jualan", tapi soal mengelola state manusia: keinginan, keputusan, dan impuls.»

Dan di sini, semuanya direduksi jadi:

localStorage

Absurd? Sedikit.
Akurat? Cukup dekat.
