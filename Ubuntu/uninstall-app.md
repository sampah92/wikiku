---
title: Uninstall program
description: menghapus instalasi pada Operasi sistem Ubuntu
published: true
date: 2020-12-27T14:36:07.341Z
tags: 
editor: markdown
dateCreated: 2020-12-18T15:33:51.834Z
---

# Uninstall
melihat aplikasi yang sudah terinstal
```
dpkg --list
```

menghapus program
`ganti "program" menggunakan nama aplikasi yang kita ketahui melalui` 
```
dpkg --list
```
```
sudo apt-get --purge remove "program"
```
