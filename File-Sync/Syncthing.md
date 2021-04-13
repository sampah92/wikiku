---
title: Syncthing
description: 
published: true
date: 2021-04-13T08:31:21.156Z
tags: 
editor: markdown
dateCreated: 2021-04-13T08:18:38.284Z
---

# Pendahuluan
[Syncthing](https://syncthing.net/) adalah program sinkronisasi berkas berkelanjutan. Ini menyinkronkan file antara dua komputer atau lebih secara real time, dilindungi dengan aman dari mata-mata. Data Anda adalah data Anda sendiri dan Anda layak untuk memilih di mana data tersebut disimpan, apakah data tersebut dibagikan dengan beberapa pihak ketiga, dan bagaimana data tersebut dikirimkan melalui internet.

# Instalasi
Program ini Portable

# Konfigurasi
- Di sebelah kiri adalah daftar "folder", atau direktori untuk disinkronkan. Anda bisa melihat Folder Default
dibuat untuk Anda, dan saat ini ditandai "Tidak Dibagikan" karena belum dibagikan dengan perangkat lain.
Di sebelah kanan adalah daftar perangkat. Saat ini hanya ada satu perangkat: komputer yang Anda jalankan ini
Pada.
- Agar Sinkronisasi dapat menyinkronkan file dengan perangkat lain, harus diberitahu tentang perangkat tersebut.
Ini dicapai dengan bertukar "ID perangkat". ID perangkat adalah id perangkat yang unik dan aman secara kriptografis
pengidentifikasi yang dihasilkan sebagai bagian dari pembuatan kunci saat pertama kali Anda memulai Syncthing. Hal ini dicetak di
log di atas, dan Anda dapat melihatnya di GUI web dengan memilih "Tindakan" (kanan atas) dan "Tampilkan ID".
- Dua perangkat hanya akan terhubung dan berbicara satu sama lain jika mereka berdua dikonfigurasi dengan perangkat satu sama lain
ID. Karena konfigurasi harus saling menguntungkan agar koneksi terjadi, ID perangkat tidak perlu disimpan
Rahasia. Mereka pada dasarnya adalah bagian dari kunci publik.
Untuk membuat kedua perangkat Anda berbicara satu sama lain klik "Tambahkan Perangkat Jarak Jauh" di kanan bawah pada keduanya,dan masukkan ID perangkat dari sisi lain. Anda juga harus memilih folder yang ingin Anda bagikan. Tje
nama perangkat bersifat opsional dan murni kosmetik. Ini dapat diubah nanti jika diperlukan.

- Setelah Anda mengklik "Simpan" perangkat baru akan muncul di sisi kanan GUI (meskipun terputus) dan
lalu sambungkan ke perangkat baru setelah satu menit atau lebih. Ingatlah untuk mengulangi langkah ini untuk perangkat lain.

Pada titik ini kedua perangkat berbagi direktori kosong. Menambahkan file ke direktori bersama baik di
perangkat akan menyinkronkan file-file tersebut ke sisi lain.
Jika Anda menggunakan ragam Syncthing yang menambahkan fungsionalitas khusus OS (misalnya aplikasi Android), y