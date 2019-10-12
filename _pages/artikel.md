---
title: Kumpulan Berita Seputar Pendidikan
description: Halaman ini berisi kumpulan artikel terupdate yang sangat berguna bagi para pembaca.
permalink: /artikel
---

<ol class="arti">{% for post in site.categories.artikel %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
