---
title: GNS3
description: simulasi jaringan internet
published: true
date: 2021-01-10T06:57:37.251Z
tags: 
editor: markdown
dateCreated: 2021-01-10T06:57:37.251Z
---

# Pendahuluan
GNS3 digunakan oleh ratusan ribu insinyur jaringan di seluruh dunia untuk meniru, mengonfigurasi, menguji, dan memecahkan masalah jaringan virtual dan nyata. GNS3 memungkinkan Anda untuk menjalankan topologi kecil yang hanya terdiri dari beberapa perangkat di laptop Anda, kepada mereka yang memiliki banyak perangkat yang dihosting di beberapa server atau bahkan dihosting di cloud.
# Instalasi
- Lakukan
```shell
sudo add-apt-repository ppa:gns3/ppa
sudo dpkg --add-architecture i386
sudo apt update
sudo apt -y install gns3-gui gns3-iou gns3-server virtualbox qemu wireshark libpcap-dev git ubridge
sudo chmod 777 /usr/bin/dumpcap
```
- Proses instalasi di atas akan secara automatis menginstall ubridge. Ubridge dari ubuntu tampaknya tidak stabil. Tampaknya masih lebih baik compile ubridge sendiri sebagai berikut,
```shell
sudo su
apt -y install libpcap-dev git
cd /usr/local/src
rm -Rf /usr/local/src/ubridge/
git clone git://github.com/GNS3/ubridge.git
cd ubridge
make
make install
cp -p ubridge /usr/bin
setcap cap_net_admin,cap_net_raw=ep /usr//bin/ubridge
```

- Tiga (3) line terakhit akan menimpa ubridge hasil dari apt install.
Selanjutnya, sebagai user biasa, siapkan directory
```shell
mkdir -p ~/GNS3/projects
mkdir -p ~/GNS3/images
```
- menjalankan
```shell
gns3 &
```
# Konfigurasi
Konfigurasi pertama kali

- Pilih

`Run appliances on my local computer`
- Klik 2
```
Server Path  : /usr/bin/gns3server
Host binding : localhost
Port         : 3080 TCP
```
- Klik 3

Pastikan

`Connection to the local GNS3 server has been successful!`
- FINISH

`Finish`