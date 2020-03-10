---
title: Kumpulan Dongeng Anak
description: Halaman ini berisi kumpulan Buku Dongeng Anak.
permalink: /dongeng
---

<ol class="arti">{% for post in site.categories.dongeng %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
