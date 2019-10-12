---
title: "Kontributor"
description: "Berikut ini adalah daftar orang-orang yang telah berkontribusi di Administrasi.Net. Bergabung bersama kami"
layout: nosidebar
---

<div class="row">
    {% for author in site.authors %}
    <div class="col-xs-12 col-sm-6 col-md-4">
        <div class="image-flip" ontouchstart="this.classList.toggle('hover');">
            <div class="mainflip">
                <div class="frontside">
                    <div class="card">
                        <div class="card-body text-center">
                            <p><img alt="{{ author[1].name }}" src="{{site.url}}{{ author[1].avatar }}" class="rounded-circle" height="80" width="80"></p>
                            <h4 class="card-title"> {{ author[1].name }}</h4>
                            <p class="card-text">{{ author[1].bio | strip_html | strip_newlines | truncate: 100 }}</p>
                            <a href="#" class="btn btn-primary btn-sm"><i class="fa fa-plus"></i></a>
                        </div>
                    </div>
                </div>
                <div class="backside">
                    <div class="card">
                        <div class="card-body text-center mt-4">
                            <h2 class="card-title"> {{ author[1].name }}</h2>
                            <p class="card-text">{{ author[1].bio }}</p>
                             <a href="{{site.url}}/{{ author[1].slug }}">View Post</a>
                            <ul class="list-inline">
                                <li class="list-inline-item">
                                    <a class="social-icon text-xs-center" target="_blank" href="https://www.facebook.com/{{ author[1].facebook }}">
                                        <i class="fa fa-facebook"></i>
                                    </a>
                                </li>
                                <li class="list-inline-item">
                                    <a class="social-icon text-xs-center" target="_blank" href="https://twitter.com/{{ author[1].twitter }}">
                                        <i class="fa fa-twitter"></i>
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    {% endfor %}
</div>
