---
layout: default
title: Pulications
permalink: ./publications.html 
# permalink: /team/
---

<section  >
    <ul>
        {% for item in site.data.publications reversed %}
            <li>{{item.Authors}} <strong>{{item.Title}}</strong>, {{item.Publication}}, {{item.Year}}</li>
        
        {% endfor %}
    </ul>
</section>