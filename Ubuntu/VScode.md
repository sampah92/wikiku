---
title: Visual Studio Code
description: menginstall Visual Studio Code di Ubuntu 20.04
published: true
date: 2020-12-22T14:21:42.153Z
tags: ubuntu, visual studio code, editor, ubuntu 20.04
editor: markdown
dateCreated: 2020-12-18T14:46:04.150Z
---

# Konfigurasi repository

lakukan
```
sudo apt update
```

install package dari microsoft
```
sudo apt install -y curl apt-transport-https
```

GPG key microsoft
```
curl -sSL https://packages.microsoft.com/keys/microsoft.asc -o microsoft.asc
sudo apt-key add microsoft.asc
```
menambah repository microsoft vscode
```
echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"  | sudo tee /etc/apt/sources.list.d/vscode.list
```

# Install VScode
Update repository
```
sudo apt update
```
install vscode
```
sudo apt install -y code
```

# Menjalankan VScode
jalankan perintah ini pada directory project
```
code .
```