---
title: DroidCam
description: ponsel menjadi webcam
published: true
date: 2021-01-02T14:02:49.472Z
tags: 
editor: markdown
dateCreated: 2021-01-02T14:02:49.472Z
---

# Pendahuluan
DroidCam mengubah perangkat seluler Anda menjadi webcam untuk PC Anda.

# Instalasi
Ubuntu 20.04 64bit

```shell
cd /tmp/
wget https://files.dev47apps.net/linux/droidcam_latest.zip
unzip droidcam_latest.zip -d droidcam
cd droidcam && sudo ./install-client
```
- Video
```shell
sudo apt install linux-headers-`uname -r` gcc make
sudo ./install-video
```
- sound
```shell
sudo ./install-sound
```
