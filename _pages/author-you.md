---
title: "You"
permalink: "/author-you"
---
<div class="container">
<div class="row justify-content-center">
    <div style="margin-top:30px">        
        <div class="row align-items-center mb-5">
            <div class="col-md-9">
                <h2 class="font-weight-bold">{{page.title}} <span class="ml-3 small btn btn-outline-success btn-sm btn-round"><a href="https://twitter.com/{{ site.authors.artipedia.twitter }}">Follow</a></span></h2>
                <p><a href="{{ site.authors.artipedia.site }}">{{ site.authors.artipedia.site }}</a></p>
                <p class="excerpt">{{ site.authors.artipedia.bio }}</p>
            </div>
            <div class="col-md-3 text-right">
                <img alt="{{ site.authors.artipedia.name }}" src="{{site.url}}{{ site.authors.artipedia.avatar }}" class="rounded-circle" height="100" width="100">
            </div>
        </div>
        <h4 class="font-weight-bold spanborder"><span>Posts by {{page.title}}</span></h4>
            {% assign posts = site.posts | where:"author","artipedia" %}
            {% for post in posts %}
            {% include main-loop-card.html %}
            {% endfor %}
    </div>
</div>
</div>
