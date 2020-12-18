---
title: Visual Studio Code
description: menginstall Visual Studio Code di Ubuntu
published: true
date: 2020-12-18T14:49:15.949Z
tags: ubuntu, visual studio code, editor
editor: markdown
dateCreated: 2020-12-18T14:46:04.150Z
---

# Konfigurasi repository
lakukan
<kbd>sudo apt update</kbd>

install package dari microsoft
<kbd>sudo apt install -y curl apt-transport-https</kbd>

GPG key microsoft
<kbd>curl -sSL https://packages.microsoft.com/keys/microsoft.asc -o microsoft.asc</kbd>

<kbd>sudo apt-key add microsoft.asc</kbd>

menambah repository microsoft vscode
<kbd>echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"  | sudo tee /etc/apt/sources.list.d/vscode.list</kbd>

# Install VScode
Update repository
<kbd>sudo apt update</kbd>

install vscode
<kbd>sudo apt install -y code</kbd>

# Menjalankan VScode
jalankan perintah ini pada directiry project
<kbd>code .</kbd>