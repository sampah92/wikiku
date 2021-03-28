---
title: Integrasi C++ di VSCODE
description: Menjalankan program C++ di VSCOde
published: true
date: 2021-03-28T16:18:52.287Z
tags: 
editor: markdown
dateCreated: 2021-03-28T16:18:52.287Z
---

# Pendahuluan
Metode ini Berguna bagi kamu yang ingin belajar C++ 

# Mingw
Download [Mingw](https://bit.ly/mingw10)

- Download mingw Tanpa Git supaya cepat
- Ekstrak di `C:/`
- Konfigurasi Gcc System Variable :
	- Masuk ke folder mingw -> bin
  - Buka System variable
  - Klik New
  - Masukan Direktori `C:\MinGW\bin`
  - Klik `Ok`
  - Verifikasi apakah gcc sudah terinstall di Command prompt dengan syntax
  ``` cmd
  g++ --version
  ```
# Visual Studio Code
- Download dan Install [visual studio code](https://code.visualstudio.com/)
  - Tambah Ekstension :
    - Code runner
    - C/C++ Intellisense
- Integrasi Terminal
  - Klik File
  - Preference
  - Setting
  - Pada Search bar ketik `run in terminal`
  - Scroll kebawah dan centang pada `code-runner: Run in Terminal`
