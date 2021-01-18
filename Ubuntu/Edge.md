---
title: Microsoft Edge
description: browser yang dikembangkan oleh microsoft
published: true
date: 2021-01-18T12:25:56.673Z
tags: 
editor: markdown
dateCreated: 2021-01-18T12:23:26.533Z
---

# instalasi
Ubuntu 20.04 (Focal)
```shell
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/edge stable main" > /etc/apt/sources.list.d/microsoft-edge-dev.list'
sudo rm microsoft.gpg
sudo apt update
sudo apt install microsoft-edge-dev
```