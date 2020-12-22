---
title: Nvidia Driver
description: menginstall GPU Driver pada Ubuntu 20.04
published: true
date: 2020-12-22T14:14:28.324Z
tags: vga, nvidia, gpu, driver, ubuntu 20.04
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
```
sudo shutdown -r now
```
atau
```
sudo reboot
```

# instalasi CLI
tapi ini lebih mudah :smile:

```
sudo Ubuntu-drivers devices
sudo ubuntu-drivers autoinstall
sudo apt install nvidia-driver-390
```
agar mengetahui perbedaanya reboot perangkat

```
sudo shutdown -r now
```

# Verifikasi
mengetahui hardware yang sudah terinstall
```
nvidia-smi
```
untuk mengubah beberapa pengaturan
```
sudo nvidia-settings
```

