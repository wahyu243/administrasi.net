---
title: Kumpulan Teori
description: Halaman ini berisi kumpulan teori yang sangat berguna bagi para pembaca.
---

<ol class="arti">{% for post in site.categories.teori %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
