---
title: Remote origin already exists
description: kendala dalam push repo ke github
published: true
date: 2020-12-27T14:34:19.433Z
tags: 
editor: markdown
dateCreated: 2020-12-22T20:42:51.852Z
---

# Kode error
`ssh: Could not resolve hostname https: Temporary failure in name resolution
fatal: Could not read from remote repository.`

`Please make sure you have the correct access rights
and the repository exists.`

# Cara pertama
generate ssh key
```
ssh-keygen -t rsa
```
buka di
```
/root/.ssh/id_rsa.pub
```
salin ke
https://github.com/settings/ssh
# Cara Kedua
```
git remote set-url origin https://github.com/your/repository
```