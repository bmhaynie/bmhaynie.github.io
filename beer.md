---
layout: base
title: Beer
permalink: /beer/
---

<section id="beer" class="bg-light-gray">
    <div class="container">
        <div class="row text-center">
            <div class="col-xs-12">
                <h2 class="section-heading">All Beer</h2>
            </div>
            <div class="col-sm-10 col-sm-offset-1">
                <p class="lead">Lorem ipsum dolor sit amet consectetur adipiscing elit. Etiam eget elementum dui in ornare est.<span class="hidden-sm hidden-xs">Click on</span><span class="hidden-lg hidden-md">Tap</span> each photo for more details.</p>
            </div>
        </div>
        <div class="row">
            {% for beer in site.beer %}
                <div class="col-lg-3 col-md-4 col-sm-6 col-xs-12 beer-item">
                    <a href="/#{{ beer.modal-id }}" class="beer-link" data-toggle="modal">
                        <div class="beer-hover">
                            <div class="beer-hover-content">
                                <i class="fa fa-search-plus fa-3x"></i>
                            </div>
                        </div>
                        <img src="/img/beer/{{ beer.img }}" class="img-responsive img-centered" alt="">
                    </a>
                    <div class="beer-caption">
                        <h3>{{ beer.name }}</h3>
                        <p class="text-muted">{{ beer.style }}</p>
                        <p><span>{{ beer.abv }}</span></p>
                    </div>
                </div>
            {% endfor %}
        </div>
    </div>
</section>