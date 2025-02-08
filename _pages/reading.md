---
title: "读书笔记"
layout: collection
permalink: /reading/
collection: reading
entries_layout: grid
classes: wide
author_profile: true
sort_by: date
sort_order: reverse
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/books/reading-banner.jpg
  overlay_filter: 0.5
excerpt: >
  阅读是一场心灵的旅行，这里记录了我在书海中的点点滴滴。
feature_row:
  - image_path: /assets/images/books/recent-1.jpg
    alt: "最新阅读"
    title: "最近在读"
    excerpt: "分享最近阅读的书籍和感想。"
---

{% include feature_row %}

<div class="grid__wrapper">
  {% assign reading = site.reading | sort: 'date' | reverse %}
  {% for post in reading %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div> 