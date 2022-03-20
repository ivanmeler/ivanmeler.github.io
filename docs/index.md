---
layout: default
title: LineageOS builds for Samsung Exynos 8890/8895 devices
---

# LineageOS builds for Samsung Exynos 8890/8895 devices

{% assign sorted_pages = site.pages | sort: 'order' %}

{% for page in sorted_pages %}
{% if page.title and page.url and page.url contains "/devices/" %}
- [{{ page.title }} ({{ page.codename }})]({{ page.url | relative_url }})
{% endif %}
{% endfor %}

{% include paypal.md %}