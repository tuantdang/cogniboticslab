---
layout: default
title: {{ site.title }}
permalink: ./index.html 
---



<div class="hero-banner ">
<div class="hero-overlay">
    <h1 style="    font-size: 1.4em;">{{site.title}}</h1>
    <p>{{site.description}} </p>
</div>
</div>

<section class="news">
    <h2>News & Events</h2>
    <ul>
        {% for item in site.data.news %}
            {% if item.link%}
            <li><strong>{{item.date}} : </strong> <a href="{{item.link}}"> {{ item.event }}</a></li>
            {% else %}
            <li><strong>{{item.date}} : </strong> {{ item.event }}</li>
            {% endif %}
        {% endfor %}
    </ul>
</section>
<!-- {% assign page = "index" %} -->