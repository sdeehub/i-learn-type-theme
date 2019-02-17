---
layout: post
title: "ร้องโน้ตเป็นตัวๆ ไม่ดึง"
date: 2019-02-17 19:10:38
feature-img: "https://res.cloudinary.com/sdees-reallife/image/upload/v1550405551/Screenshot_from_2019-02-17_19-12-10.png"
credit-name:
credit-user:
tags:
- Coding
---
วันนี้ได้เรียนรู้ YAML ตอนที่เราแก้ไฟล์ใน Jekyll มีอยู่ 2 ส่วนที่ง่ายๆ ตามนี้เลย:

`{% assign sorted = (site.tags[this_word] | sort) %}`

อันนี้เอาไว้ Sort - กับอีกอัน

`{{ paginator.previous_page_path | relative_url }}`

อันนี้เอาไว้อ้าง Relative_URL
