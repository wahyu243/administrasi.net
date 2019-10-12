---
title: Kumpulan Tutorial
description: Halaman ini berisi kumpulan tutorial yang sangat berguna bagi para pembaca.
permalink: /tutorial
---

<ol class="arti">{% for post in site.categories.tutorial %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
