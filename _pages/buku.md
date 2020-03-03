---
title: Kumpulan Buku Sekolah Digital (BSD)
description: Halaman ini berisi kumpulan Buku sekolah SD, SMP, SMA, dll terdiri dari buku guru, buku siswa, komik pendiikan yang sangat berguna bagi para pembaca.
permalink: /bsd
redirect_from: /buku
---

<ol class="arti">{% for post in site.categories.buku %}
<li class="{% if page.title == post.title %}current{% endif %}">
<a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
</li>
{% endfor %}
</ol>
