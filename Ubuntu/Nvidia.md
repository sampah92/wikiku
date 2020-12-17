---
title: Nvidia Driver
description: menginstall GPU Driver pada Ubuntu
published: true
date: 2020-12-17T12:58:54.806Z
tags: vga, nvidia, gpu, driver
editor: markdown
dateCreated: 2020-12-15T19:46:35.830Z
---

# instalasi GUI
lebih mudah menggunakan GUI

buka

`software and updates`
`pilih driver yang cocok`
`Apply change`


lalu restart
<kbd>sudo shutdown -r now</kbd>
atau
<kbd>sudo reboot</kbd>

# instalasi CLI
tapi ini lebih mudah :smile:

<kbd>sudo Ubuntu-drivers devices</kbd>
<kbd>sudo ubuntu-drivers autoinstall</kbd>
<kbd>sudo apt install nvidia-driver-390</kbd>

agar mengetahui perbedaanya reboot perangkat

<kbd>sudo shutdown -r now</kbd>

# Verifikasi
mengetahui hardware yang sudah terinstall
<kbd>nvidia-smi</kbd>

untuk mengubah beberapa pengaturan
<kbd>sudo nvidia-settings</kbd>