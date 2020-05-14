---
title: Kumpulan Tutorial
description: Halaman ini berisi kumpulan tutorial, cara atau konten panduan cara yang paling andal, lengkap, dan menyenangkan di internet.
permalink: /tutorial
---

<ol class="arti">{% for post in site.categories.tutorial %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
