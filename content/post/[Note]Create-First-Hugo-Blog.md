---
title: "[Note] Create First Hugo Blog"
date: 2025-08-29T10:00:00+08:00
draft: false
description: "Note for process of buiding the static blog."
tags: ["hugo","blog","Note"]
categories: ["blog"]
---

## Why I Started This Blog
I wanted a place to ducument both my technical journey and personal growth.

---

### Notes on Building This Blog
This is my very first attempt at creating a Hugo static site.  
I'll keep it simple for now - just recording the steps I took.  
Maybe in the future,when I learn more,I'll come back and add more details.

---

#### Getting Started
My test/lab environment  
OS：windows 11  
WSL：Ubutun(works inside WSL’s Linux filesystem,e.g.,~/sites)  

```markdown
1. Install HUGO  
Install Hugo extended(x86_64/amd64)
Commands(preferred: .deb install)
   ```bash
   # Remove any old distro Hugo
   sudo apt remove -y hugo   
   # Copy the correct package (from your Windows Downloads) into WSL home
   cp /mnt/c/Users/<YOU>/Downloads/hugo_extended_*_linux-amd64. deb ~/
   # Fix perms (optional safety)
   chmod 644 ~/hugo_extended_*_linux-amd64.deb
   # Install
   sudo apt install -y ./hugo_extended_*_linux-amd64.deb
   # Verify
   hugo version   # expect: hugo v0.128+ *+extended* linux/amd64
   ```
2. Create Site(in WSL)
keep the project in Linux FS for speed and fewer path issues.
```bash
mkdir -p ~/sites
cd ~/sites
hugo new site myblog
cd myblog
```

---

*For now, this is just a starting point. Future me can fill in the blanks when I know more.*  