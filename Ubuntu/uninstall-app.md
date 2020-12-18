---
title: Uninstall program
description: menghapus instalasi pada Operasi sistem Ubuntu
published: true
date: 2020-12-18T15:33:51.834Z
tags: ubuntu, uninstall, hapus
editor: markdown
dateCreated: 2020-12-18T15:33:51.834Z
---

# Uninstall
melihat aplikasi yang sudah terinstal
<kbd>dpkg --list</kbd>

menghapus program
`ganti "program" menggunakan nama aplikasi yang kita ketahul melalui` <kbd>dpkg --list</kbd>
<kbd>sudo apt-get --purge remove "program"</kbd>
