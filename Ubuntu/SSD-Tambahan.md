---
title: SSD Ubuntu
description: Merubah permission Drive pada Ubuntu 20.04
published: true
date: 2020-12-27T14:35:41.786Z
tags: 
editor: markdown
dateCreated: 2020-12-15T18:01:13.676Z
---

# SSD Permission
merubah read and write drive.
saat menggunakan perintah ini kebetulan berhasil

cari tahu dulu nama Drivenya

```
sudo fdisk -l
```
lalu
```
sudo ntfsfix /dev/your_drive
```



