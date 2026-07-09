---
layout: home
title: Horizon Daily
---

# 🌅 Horizon Daily

> AI 驱动的每日资讯雷达 | AI+教育 · 地理教育

{% assign posts = site.posts | sort: "date" | reverse %}

## 📰 最新日报

{% for post in posts limit: 10 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

---

*每日自动更新 · Powered by [Horizon](https://github.com/Thysrael/Horizon)*
