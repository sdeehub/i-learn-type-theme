---
layout: post
title: "Blogger to Jekyll"
date: 2019-03-21 15:00:00 +0700
feature-img: "https://source.unsplash.com/5eBW5GomfhY"
credit-name: "Irvan Smith"
credit-user: "@mr_vero"
tags:
- Reference
---
กำลังจะย้าย Post ที่ค้างอยู่ที่ Blogger ไป Jekyll - มีรายละเอียดตามนี้:
- [Backup Blogger](https://support.google.com/blogger/answer/41387?hl=en)
- [Blogger to Jekyll](https://import.jekyllrb.com/docs/blogger/)

```bash
$ ruby -r rubygems -e 'require "jekyll-import";
    JekyllImport::Importers::Blogger.run({
      "source"                => "/path/to/blog-MM-DD-YYYY.xml",
      "no-blogger-info"       => false, # not to leave blogger-URL info (id and old URL) in the front matter
      "replace-internal-link" => false, # replace internal links using the post_url liquid tag.
    })'
```

*Status*: ยังไม่สำเร็จ น่าจะมาจาก UTF-8 หรืออะไรสักอย่างในไฟล์ XML
