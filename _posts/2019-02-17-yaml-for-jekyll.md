---
layout: post
title: "เรียน YAML ไปนิดหน่อย"
date: 2019-02-17 19:10:38
feature-img: "https://res.cloudinary.com/sdees-reallife/image/upload/v1550405551/Screenshot_from_2019-02-17_19-12-10.png"
tags:
- Coding
---
วันนี้ได้เรียนรู้ YAML ตอนที่เราแก้ไฟล์ใน Jekyll มีอยู่ 2 ส่วนที่ง่ายๆ ตามนี้เลย:


อันนี้เอาไว้ Sort - กับอีกอัน

```html
{% assign sorted = (site.tags[this_word] | sort) %}
{% for post in sorted %}{% if post.title != null %}
<div class="tag-list">
    <span><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></span>
    <small><span>| {{ post.date | date_to_string }}</span></small>
</div>
{% endif %}{% endfor %}
```

อันนี้เอาไว้อ้าง Relative_URL
