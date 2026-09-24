---
layout: karya
title: MYHOME (Sistem Smart Home Otomasi)
slug: myhome
author: Fuja Bungsu Ali Nawawi
author_link: '#'
author_image: '#'
category: IoT
event_tag: Galaksi 2026
hero_image: /assets/images/karya/myhome/myhome_1.webp
description: Prototype sistem otomasi rumah pintar berbasis mikrokontroler sensor
  gerak, suhu, dan cahaya terintegrasi relay lampu.
contributors: Fuja Bungsu Ali Nawawi, Galih Pratama
tech_stack:
- ESP32 / Arduino
- Embedded C++
- Relay Module
- PIR Sensor
- IoT
gallery:
- image: /assets/images/karya/myhome/myhome_1.webp
  caption: Display Prototype Rangkaian MYHOME di Pameran
- image: /assets/images/karya/myhome/myhome_2.webp
  caption: Wiring Mikrokontroler & Modul Sensor
- image: /assets/images/karya/myhome/myhome_3.webp
  caption: Pengujian Respon Relay & Indikator Output
---

### Ringkasan Proyek
**MY[HOME]** adalah prototipe sistem *smart home* (rumah pintar) berbasis mikrokontroler dan *Internet of Things* yang dikembangkan oleh **Divisi RIOT (Republic Internet of Things)** sebagai solusi kendali hunian modern yang hemat energi dan aman.

### Mekanisme Kerja
1. **Input (Sensor):** Mendeteksi keberadaan penghuni melalui sensor PIR, membaca suhu ruangan, dan intensitas cahaya matahari.
2. **Processing:** Mikrokontroler mengevaluasi kondisi ambang batas (*threshold*) lingkungan secara real-time.
3. **Output (Aktuator):** Memicu relay untuk menyalakan/mematikan lampu dan membunyikan alarm keselamatan jika terdeteksi anomali.
