# Panduan Menambahkan Karya Baru di Website RIT Expo

Dokumen ini berisi panduan langkah demi langkah bagi pengurus dan kontributor UKM Republic of Information Technology (RIT) untuk menambahkan karya inovasi baru ke dalam katalog web **FKOMINFO EXPO**.

---

## 🚀 Alur Singkat (3 Langkah Mudah)

1. **Langkah 1:** Siapkan foto/screenshot karya di folder `assets/images/karya/<slug-karya>/`.
2. **Langkah 2:** Salin file `_karya/_template.md` menjadi `_karya/<slug-karya>.md`, lalu lengkapi isinya.
3. **Langkah 3:** Daftarkan `<slug-karya>` ke dalam file `_data/event.yml`.

---

## 📁 Langkah 1: Menyiapkan Aset Foto & Dokumentasi

1. Buat folder baru di dalam direktori gambar:
   ```bash
   assets/images/karya/<slug-karya>/
   ```
   *Contoh:* `assets/images/karya/smart-greenhouse/`

2. Masukkan file foto yang dibutuhkan:
   * **`cover.webp`** (atau `.jpg` / `.png`): Foto utama yang menjadi thumbnail di kartu beranda dan banner header di halaman detail (rekomendasi rasio `16:9` atau `16:10`, resolusi lebar minimal 1280px).
   * **Foto Galeri Dokumentasi:** Foto-foto pendukung untuk galeri WhatsApp Lightbox (misal `alat_1.webp`, `antarmuka.webp`, `pameran.webp`).
   * *Tips:* Gunakan format `.webp` agar ukuran gambar ringan dan web dimuat sangat cepat tanpa mengurangi ketajaman visual.

---

## 📝 Langkah 2: Membuat File Dokumen Karya

1. Salin template yang sudah disediakan di `_karya/_template.md` menjadi file baru dengan format nama `<slug-karya>.md`.
   *Contoh:* `_karya/smart-greenhouse.md`
   *(Catatan: Gunakan huruf kecil tanpa spasi, pisahkan kata dengan tanda hubung `-`)*.

2. Buka file tersebut dan sesuaikan bagian **Frontmatter** (bagian di antara tanda `---` di paling atas):

```yaml
---
layout: karya
title: "Smart Greenhouse Monitoring"     # Judul resmi karya
slug: "smart-greenhouse"                 # Wajib SAMA dengan nama file tanpa .md
author: "Nama Pembuat"                   # Nama pengembang utama
author_link: "https://github.com/..."    # Link profil author (atau '#' jika tidak ada)
author_image: "#"                        # URL foto profil (atau '#' untuk inisial)
contributors: "Nama Rekan 1, Nama Rekan 2" # Opsional: Kontributor tim lainnya

# Kategori resmi (Pilih salah satu agar warna badge semantik sesuai):
# - Web (Badge Biru)
# - IoT (Badge Hijau Emerald)
# - Game (Badge Ungu)
# - Cyber Security (Badge Merah Rose)
category: "IoT"

# Label event debut / pameran
event_tag: "Galaksi 2026"

# Path gambar sampul utama
hero_image: "/assets/images/karya/smart-greenhouse/cover.webp"

# Deskripsi ringkas untuk kartu depan (1-2 kalimat padat)
description: "Sistem otomasi pemantauan suhu, kelembapan, dan penyiraman tanaman cerdas berbasis mikrokontroler ESP32."

# Link Aksi (Pilih yang relevan):
demo_link: "https://greenhouse.uniga.ac.id" # Link live web / aplikasi (opsional)
demo_label: "Buka Dashboard Live"          # Label kustom tombol demo

repo_link: "https://github.com/RIT-Base/smart-greenhouse" # Link repositori GitHub (opsional)

# Chip tag teknologi di sidebar
tech_stack:
  - "ESP32"
  - "MicroPython"
  - "MQTT"
  - "Tailwind CSS"

# Galeri Foto Interaktif (WhatsApp-Style Lightbox)
gallery:
  - image: "/assets/images/karya/smart-greenhouse/alat_1.webp"
    caption: "Unit instalasi sensor kelembapan tanah dan mikrokontroler di perkebunan"
  - image: "/assets/images/karya/smart-greenhouse/dashboard.webp"
    caption: "Tampilan dashboard web pemantauan suhu dan grafik telemetri real-time"
---
```

3. Tuliskan deskripsi lengkap karya di bagian bawah frontmatter menggunakan format Markdown:
   * `### Ringkasan Produk`
   * `### Fitur Unggulan`
   * `### Cara Kerja & Arsitektur`
   * `### Catatan Pameran / Prestasi`

---

## ⚙️ Langkah 3: Mendaftarkan Karya ke `_data/event.yml`

Agar karya yang baru dibuat muncul di halaman Beranda, buka file `_data/event.yml`:

```yaml
# Info Event yang Sedang Berlangsung
current_name: "Katalog Karya Unggulan RIT"
current_desc: "Pameran inovasi teknologi, robotika IoT, aplikasi web, dan game karya mahasiswa RIT FKOMINFO UNIGA."
status: "active"

# 1. CAROUSEL UNGGULAN (Slider besar paling atas di beranda)
# Masukkan slug karya jika ingin ditampilkan sebagai highlight utama:
carousel_karya:
  - "mozybit"
  - "rit-oms"
  - "smart-greenhouse"  # <--- Tambahkan di sini jika karya unggulan

# 2. SEDANG TAMPIL (Grid katalog karya di bawah carousel)
# Masukkan slug karya agar kartu karyanya muncul di beranda dan arsip pencarian:
current_karya:
  - "mozybit"
  - "rit-oms"
  - "smart-greenhouse"  # <--- Tambahkan slug karya baru di sini!
  - "ctf-uts-fkom"
  - ...
```

---

## 🔍 Cara Menguji di Komputer Lokal

1. Buka terminal atau Command Prompt (CMD) di folder proyek `D:\github\Expo`.
2. Jalankan perintah pembangunan atau server lokal:
   ```bash
   bundle exec jekyll serve
   # atau jika menggunakan jekyll langsung:
   jekyll serve
   ```
3. Buka peramban (browser) di alamat `http://localhost:4000/Expo/`.
4. Pastikan:
   * Kartu karya muncul di Beranda dengan warna semantik kategori yang tepat.
   * Filter pencarian dan tombol kategori berfungsi lancar.
   * Halaman detail dapat dibuka dan tombol aksi (Demo / GitHub) mengarah ke link yang benar.
   * Foto-foto di galeri dokumentasi dapat diklik untuk membuka **WhatsApp Lightbox Viewer** (coba tombol panah, klik thumbnail di bawah, dan coba tombol `ESC` untuk menutup).

---

*Selamat berkarya dan memamerkan inovasi terbaik mahasiswa RIT FKOMINFO UNIGA!* 🚀✨
