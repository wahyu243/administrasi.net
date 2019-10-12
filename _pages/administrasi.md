---
title: Kumpulan administrasi
description: Halaman ini berisi kumpulan administrasi terupdate yang sangat berguna bagi para pembaca.
permalink: /administrasi
---

<ol class="arti">{% for post in site.categories.administrasi %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
