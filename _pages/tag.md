---
layout: page
permalink: /tag
title: Tag
description: Halaman ini berisi posting yang dikelompokkan kembali menjadi beberapa tags.
---

<

Halaman ini berisi posting yang dikelompokkan berdasarkan tag tertentu
<div id="archives">
{% for tag in site.tags %}
  <div class="archive-group">
    {% capture tag_name %}{{ tag | first }}{% endcapture %}
    <div id="#{{ tag_name | slugize }}"></div>
    <p></p>
    
    <h3 class="category-head"><i class="fa fa-tags" aria-hidden="true"></i> {{ tag_name }}</h3>
    <a name="{{ tag_name | slugize }}"></a>
    <ol class="arti">
      {% for post in site.tags[tag_name] %}
          <li><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></li>
       {% endfor %}
       </ol>
  </div>
{% endfor %}
</div>
