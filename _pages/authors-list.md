---
title: "Kontributor"
permalink: "/authors-list"
---

<div class="container">
<div class="row gap-y listrecent listrecent listauthor">
    {% for author in site.authors %}
        <div class="item-author">
            <div class="pt-4 border rounded">
            <div class="row">
            <div class="col-md-3 mb-4 mb-md-0"><img alt="{{ author[1].name }}" src="{{site.url}}{{ author[1].avatar }}" class="rounded-circle" height="80" width="80"></div>
            <div class="col-md-9">
            <a href="{{site.url}}/author-{{ author[1].slug | slugify }}">
            <h2 class="text-dark mb-0" style="text-transform: capitalize;"> {{ author[1].name }} </h2> </a>
             <a href="{{site.url}}/author-{{ author[1].slug | slugify }}">
                 <small class="d-inline-block mt-1 mb-3 font-weight-normal">(View Posts)</small></a>
            <div class="excerpt">{{ author[1].bio }}</div>
            <div class="icon-block mt-3 d-flex justify-content-between">  
            <div>
            <a target="_blank" href="https://twitter.com/{{ author[1].twitter }}"><i class="fa fa-twitter text-muted" aria-hidden="true"></i></a>  &nbsp;
            <a target="_blank" href="{{ author[1].site }}"><i class="fa fa-globe text-muted" aria-hidden="true"></i></a> &nbsp; 
                <a target="_blank" href="https://www.facebook.com/{{ author[1].facebook }}"><i class="fa fa-facebook text-muted" aria-hidden="true"></i></a> &nbsp;
            </div>
            </div>
            </div>
            </div>
            </div>
        </div>
    {% endfor %}
    </div>
</div>
