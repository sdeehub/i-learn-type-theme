---
title: MacOS
date: 2020-02-16 14:26:23 Z
tags:
- Practicing
layout: post
feature-img: https://res.cloudinary.com/sdees-reallife/image/upload/v1555658919/sample_feature_img.png
---

MacOS + NTFS = Not working!

<i class="fa fa-child" style="color:plum"></i>

Elementary OS - The fast, open, and privacy-respecting replacement for Windows and macOS.

*เวลาที่ wifi ยังใช้ไม่ได้*

- sudo apt-get remove --purge bcmwl-kernel-source
- sudo apt-get install firmware-b43-installer b43-fwcutter
- sudo nano /etc/modprobe.d/blacklist.conf : ใส่ comment ที่ bcm43xx
