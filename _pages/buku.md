---
title: Kumpulan Buku Sekolah Elektronik (BSE)
description: Halaman ini berisi kumpulanBuku Sekolah Elektronik (BSE) SD, SMP, SMA, dll terdiri dari buku guru, buku siswa, komik pendidikan yang sangat berguna bagi para pembaca.
permalink: /bse
---

<ol class="arti">{% for post in site.categories.buku %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
