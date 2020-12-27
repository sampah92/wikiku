---
title: Deploy hugo
description: deploy hugo ke github
published: true
date: 2020-12-27T14:37:50.711Z
tags: 
editor: markdown
dateCreated: 2020-12-22T21:12:59.648Z
---

# Konfig shell
simpan perintah ini lalu jalankan didalam direktori hugo
simpan dengan format .sh contoh `deploy.sh`
```shell
#!/bin/sh

# If a command fails then the deploy stops
set -e

printf "\033[0;32mDeploying updates to GitHub...\033[0m\n"

# Build the project.
hugo # if using a theme, replace with `hugo -t <YOURTHEME>`

# Go To Public folder
cd public

# Add changes to git.
git add .

# Commit changes.
msg="rebuilding site $(date)"
if [ -n "$*" ]; then
	msg="$*"
fi
git commit -m "$msg"

# Push source and build repos.
git push origin main
```
buka terminal pada direktori ini lalu jalankan perintah
```shell
./deploy.sh
```

