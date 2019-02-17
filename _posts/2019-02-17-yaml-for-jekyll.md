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

```YAML
{% assign sorted = (site.tags[this_word] | sort) %}
{% for post in sorted %}{% if post.title != null %}
<div class="tag-list">
    <span><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></span>
    <small><span>| {{ post.date | date_to_string }}</span></small>
</div>
```
อันนี้เอาไว้ Sort - กับอีกอัน

```YAML
<div class="pagination clearfix">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path | relative_url }}" class="previous"><i class="fa fa-angle-left" aria-hidden="true"></i> Previous</a>
  {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path | relative_url }}" class="next">Next <i class="fa fa-angle-right" aria-hidden="true"></i></a>
  {% endif %}
</div>
```
อันนี้เอาไว้อ้าง Relative_URL
