---
title: Nvidia Driver: install
description: 
published: true
date: 2020-12-15T19:56:35.445Z
tags: vga, nvidia, gpu, driver
editor: markdown
dateCreated: 2020-12-15T19:46:35.830Z
---

# installasi GUI
lebih mudah menggunakan GUI

buka
```mermaid 
software and updates
```
```mermaid 
pilih driver yang cocok
```
```mermaid 
Apply change
```

lalu restart
<kbd>sudo shutdown -r now</kbd>
atau
<kbd>sudo reboot</kbd>

# installasi CLI
tapi ini lebih mudah :smile:

<kbd>sudo Ubuntu-drivers devices</kbd>
<kbd>sudo ubuntu-drivers autoinstall</kbd>
<kbd>sudo apt install nvidia-driver-390</kbd>

agar mengetahui perbedaanya reboot perangkat

<kbd>sudo shutdown -r now</kbd>

# Verifikasi
<kbd>nvidia-smi</kbd>

untuk mengubah beberapa pengaturan
<kbd>sudo nvidia-settings</kbd>