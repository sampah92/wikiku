---
title: SSD Ubuntu
description: Merubah permission Drive pada Ubuntu 20.04
published: true
date: 2020-12-22T14:16:37.674Z
tags: ssd, ubuntu, permission, ubuntu 20.04, drive
editor: markdown
dateCreated: 2020-12-15T18:01:13.676Z
---

# SSD Permission
saat menggunakan perintah ini kebetulan berhasil

cari tahu dulu nama Drivenya

```
sudo fdisk -l
```
lalu
```
sudo ntfsfix /dev/your_drive
```



