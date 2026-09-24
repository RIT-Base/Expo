---
# ==============================================================================
# TEMPLATE DOKUMEN KARYA RIT EXPO
# ==============================================================================
# Petunjuk:
# 1. Salin (copy) file ini dan beri nama sesuai slug karya: `_karya/<slug-karya>.md`
#    Contoh: `_karya/smart-greenhouse.md`
# 2. Isi seluruh field frontmatter di bawah ini dengan lengkap.
# 3. Masukkan slug ke dalam file `_data/event.yml` agar muncul di halaman depan.
# ==============================================================================

layout: karya
title: "Nama Karya atau Produk Inovasi"
slug: "slug-karya"                    
# Wajib huruf kecil & tanda hubung, sama persis dengan nama file tanpa .md
author: "Nama Pembuat Utama"
author_link: "https://github.com/username"   
# Link GitHub, LinkedIn, atau Instagram (gunakan '#' jika tidak ada)
author_image: "#"                            
# URL foto profil (gunakan '#' untuk memakai inisial otomatis)
contributors: "Nama Rekan 1, Nama Rekan 2"   
# Opsional: Tuliskan anggota tim lainnya jika karya kelompok

# Kategori resmi (Pilih salah satu): Web | Mobile | IoT | Game | Cyber Security
category: "Web"

# Penanda pameran/event debut (misal: Galaksi 2026, Pesta Rakyat Uniga, PKKMB 2026, Riset Internal)
event_tag: "Galaksi 2026"

# Gambar sampul utama (tampil di kartu beranda & header halaman detail)
# Simpan foto di: /assets/images/karya/<slug>/cover.webp (bisa juga format .jpg/.png atau URL eksternal)
hero_image: "/assets/images/karya/slug-karya/cover.webp"

# Ringkasan singkat untuk kartu di beranda (maksimal 1-2 kalimat padat dan informatif)
description: "Deskripsi singkat yang menjelaskan fungsi utama produk secara menarik untuk pengunjung pameran."

# Tombol Aksi Utama (Bisa link live web, marketplace, atau itch.io)
demo_link: "https://demo-aplikasi.com"
demo_label: "Buka Demo / Aplikasi"          
 # Opsional: Label kustom tombol (misal: "Mainkan di Itch.io", "Lihat di Shopee")

# Link Repositori GitHub (Jika ada, otomatis memunculkan tombol GitHub di samping tombol Demo)
repo_link: "https://github.com/RIT-Base/nama-repo"

# Daftar teknologi yang digunakan (muncul sebagai badge tags rapi di sidebar)
tech_stack:
  - "Teknologi 1"
  - "Teknologi 2"
  - "Teknologi 3"

# ==============================================================================
# GALERI DOKUMENTASI & FOOTAGE (WhatsApp-Style Interactive Lightbox)
# ==============================================================================
# Foto-foto di bawah ini otomatis interaktif: bisa diklik untuk fullscreen,
# bisa digeser (swipe di mobile, panah di desktop), dan ada thumbnail strip di bawah.
gallery:
  - image: "/assets/images/karya/slug-karya/foto_1.webp"
    caption: "Keterangan foto 1: Suasana demonstrasi alat di booth pameran"
  - image: "/assets/images/karya/slug-karya/foto_2.webp"
    caption: "Keterangan foto 2: Tampilan antarmuka dashboard monitoring"
  - image: "/assets/images/karya/slug-karya/foto_3.webp"
    caption: "Keterangan foto 3: Detail komponen mikrokontroler dan sensor"
---

### Ringkasan Produk
Tuliskan penjelasan produk secara naratif di sini. Jelaskan latar belakang masalah yang ingin diselesaikan, siapa target penggunanya, dan mengapa produk ini inovatif.

### Fitur Unggulan
Jelaskan modul dan fitur utama yang dimiliki oleh karya ini:
* **Fitur Utama 1:** Penjelasan singkat mekanisme kerja fitur ini.
* **Fitur Utama 2:** Penjelasan singkat mekanisme kerja fitur ini.
* **Fitur Utama 3:** Penjelasan singkat mekanisme kerja fitur ini.

### Cara Kerja & Arsitektur
Jika relevan, ceritakan bagaimana sistem ini beroperasi dari input hingga output:
1. **Input:** Data yang ditangkap oleh sistem (sensor, input pengguna, form, dll).
2. **Pemrosesan:** Bagaimana logika sistem atau mikrokontroler mengolah data.
3. **Output:** Hasil akhir yang diberikan kepada pengguna (tampilan layar, notifikasi, penggerak motor, dll).

### Catatan Tambahan / Prestasi
Tuliskan catatan pencapaian jika karya ini pernah memenangkan perlombaan, hak cipta/HKI, atau respon audiens saat dipamerkan di acara kampus.
