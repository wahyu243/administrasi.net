---
title: Kumpulan Berita Seputar Pendidikan
description: Halaman ini berisi kumpulan berita terupdate tentang Pendidikan, CPNS, ataupun lainnya yang sangat berguna bagi para pembaca.
permalink: /berita
---

<ol class="arti">{% for post in site.categories.berita %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
