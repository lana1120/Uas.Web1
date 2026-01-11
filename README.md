# Uas.Web1
 - *Nama   : Maulana Malik Ibrahim*
 - *Nim    : 312010185*
 - *Kelas  : TI.24.A2*
 - *Dosen  :Agung Nugroho, S.Kom., M.Kom.*
 - *Matkul : Pemrograman Web*

link : https://youtu.be/-ix-XswQz10?si=1c2AiwrH3C_TUZly


# *STRUKTUR SPAREPART LANSVARISI*
```
project-root/
│
├── admin/
│   ├── kategori/
│   │   ├── edit.php
│   │   ├── hapus.php
│   │   ├── index.php
│   │   └── tambah.php
│   │
│   ├── sparepart/
│   │   ├── uploads/
│   │   │   └── sparepart/           (folder untuk upload gambar sparepart)
│   │   ├── edit.php
│   │   ├── hapus.php
│   │   ├── index.php
│   │   └── tambah.php
│   │
│   ├── users/
│   │   ├── edit.php
│   │   ├── hapus.php
│   │   ├── index.php
│   │   └── tambah.php
│   │
│   └── dashboard.php
│
├── api/
│   ├── add_to_card.php
│   ├── clear_cart.php
│   ├── get_cart_count.php
│   ├── remove_cart.php
│   └── update_cart.php
│
├── assets/
│   ├── css/
│   │   └── style.css
│   │
│   └── js/
│       └── script.js
│
├── uploads/
│   ├── sparepart/                    (folder utama untuk upload sparepart)
│   └── users/                        (folder untuk upload gambar profil user)
│
├── config/
│   ├── constants.php
│   └── database.php
│
├── includes/
│   ├── footer.php
│   ├── functions.php
│   ├── header.php
│   └── user/
│       ├── cart.php
│       ├── dashboard.php
│       ├── profile.php
│       ├── detail_sparepart.php
│       ├── index.php
│       ├── login.php
│       ├── logout.php
│       ├── register.php
│       ├── sidebar.php
│       ├── sparepart.php
│       └── tentang.php
│
└── (root files)
    ├── index.php                      (file utama - halaman depan)
    └── [other possible root files]
```

**KETERANGAN STRUKTUR**

1. ADMIN SECTION (`/admin/`)
 - kategori/: Manajemen kategori produk/sparepart
   - `edit.php` - Edit kategori
   - `hapus.php` - Hapus kategori
   - `index.php` - Daftar kategori
   - `tambah.php` - Tambah kategori baru
 - sparepart/: Manajemen data sparepart
   - `uploads/sparepart/` - Subfolder untuk gambar sparepart
   - CRUD files untuk operasi sparepart 
 - users/: Manajemen pengguna sistem
   - CRUD files untuk operasi user
 - `dashboard.php` - Dashboard admin utama

2. API ENDPOINTS (`/api/`)
 - Semua file terkait operasi cart/shopping cart
 - `add_to_card.php` - Tambah item ke keranjang
 - `clear_cart.php` - Kosongkan keranjang
 - `get_cart_count.php` - Ambil jumlah item di keranjang
 - `remove_cart.php` - Hapus item dari keranjang
 - `update_cart.php` - Update kuantitas keranjang

3. ASSETS (`/assets/`)
 - css/: Stylesheet
   - `style.css` - File CSS utama
 - js/: JavaScript
   - `script.js` - File JavaScript utama

4. UPLOADS (`/uploads/`)
 - sparepart/: Penyimpanan gambar sparepart
 - users/: Penyimpanan foto profil pengguna

5. CONFIGURATION (`/config/`)
 - `constants.php` - Konstanta dan setting aplikasi
 - `database.php` - Koneksi database

6. INCLUDES (`/includes/`)
 - Template dan komponen reusable:
   - `header.php` - Header template
   - `footer.php` - Footer template
   - `functions.php` - Fungsi-fungsi helper
 - user/: Halaman untuk user biasa
   - Semua halaman frontend/user side

7. ROOT FILES
 - `index.php` - Halaman utama/landing page
 - File-file lainnya di root directory

# *Hasil OutPut dan Penjelasannya*

<img width="1919" height="1065" alt="image" src="https://github.com/user-attachments/assets/09bf1475-443e-4e33-84ec-b6495b859673" />

# *Halaman Login Admin*


<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/16dc265e-d6fe-4d19-b3d6-d67166c188c5" />

# *Dashboard Admin*
Sistem Sparepart Motor. Dashboard ini dirancang untuk admin mengelola sistem sparepart dengan:
 - Gambaran cepat kondisi sistem (stok, pengguna baru).
 - Akses cepat ke fitur utama (tambah, kelola).
 - Monitoring stok rendah untuk antisipasi kehabisan.
 - Melacak pengguna baru.

<img width="1920" height="1200" alt="Cuplikan layar 2026-01-11 203636" src="https://github.com/user-attachments/assets/eedb48dd-2fbc-4847-8f56-ea1348b0c24a" />
<img width="1920" height="1200" alt="Cuplikan layar 2026-01-11 203753" src="https://github.com/user-attachments/assets/7880a6d3-0431-430d-a720-23020bb7eb51" />

# *Halaman Utama / Landing Page - Toko Sparepart Motor*
**Bagian 1: Hero Section / Promo Utama**
 - Judul: "Temukan Sparepart Motor Terbaik"
 - Tagline: Menyediakan sparepart original, kualitas terbaik, harga terjangkau
 - Tombol Aksi:
   - "Belanja Sekarang"
   - "Lihat Kategori"
 - Produk Unggulan:
   - BREMBO RCS 17 (Master rem) – tampil besar sebagai promo utama
   - BILED AES VARIO 125 – lampu LED harga Rp 5.000.000

**Bagian 2: Daftar Kategori**
Tampilan cepat kategori sparepart:
 - Aksesoris
 - Kelistrikan
 - Mesin
 - Rangka & Body
 - Rem
 - Suspensi

**Bagian 3: Sparepart Terbaru**
Menampilkan produk baru berdasarkan kategori Aksesoris:

 - MASTER REM BREMBO RCS 17 – Rp 800.000 (Stok: 40)
 - BILED AES VARIO 125/150 – Rp 5.000.000 (Stok: 80)
 - PAKET BORE UP VARIO/PCX/ADV HRT – Rp 2.000.000 (Stok: 100)
 - AKI RACING LITHIUM TOR – Rp 600.000 (Stok: 40)

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/35f40573-2fe6-410d-9d34-d21d672cf6f9" />

# *Halaman Katalog Sparepart Lengkap*
Struktur Halaman:
1. Header & Branding
 - Nama Toko: "LANSVARIASI" (kemungkinan brand/toko sparepart)

2. Sidebar Filter (Kiri)
- Pencarian: "Cari Sparepart" dengan input nama sparepart
- Filter Kategori:
  - Semua Kategori
  - Akesoris (typo: seharusnya "Aksesoris")
  - Kelistrikan
  - Mesin
  - Rangka & Body
  - Rem
  - Suspensi

3. Area Produk (Tengah/Kanan)
- Info jumlah: "17 sparepart ditemukan"
- Produk ditampilkan dalam kartu (card) per item

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/35c85c62-6587-44cf-a946-e3cb9ab9aeaf" />

# *Halaman Keranjang Belanja (Kosong)*
Struktur Halaman:
1. Header & Navigasi
 - Brand: LANSVARIASI
 - Menu Navigasi:
   - Home
   - Varfasi (mungkin "Variasi" atau "Sparepart")
   - Tentang Lansvarfasi (typo: "Lansvarfasi")
   - Keranjang
   - Dashboard
   - Administrator ▼ (dropdown menu admin)

2. Sidebar Profil (Kiri)
 - Info Admin: "admin" (nama user)
 - Member sejak: 11 Jan 2028 (data contoh/future date)
 - Menu Profil:
   - Pesanan Saya
   - Keranjang Belanja (active/dicentang)
   - Wishlist
   - Alamat Saya
   - Logout

3. Area Utama Keranjang
 - Judul: "Keranjang Belanja"
 - Info: "0 item di keranjang"
 - Status: "Keranjang Belanja Kosong"
 - Pesan: "Tambahkan sparepart ke keranjang untuk melanjutkan" (typo: "spareport")
 - Tombol/Tautan: "Mulai Belanja" (link placeholder)

