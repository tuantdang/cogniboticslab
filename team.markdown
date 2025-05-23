---
layout: default
title: Team
permalink: ./team.html 
# permalink: /team/
---
<!-- <h2>Lab members</h2> -->

<section>
   {% for group in site.data.team %}
        {% if group.people.size > 0 %}
        <div class="directory_people" >
            <h4 style="margin-top: 10px; margin-bottom: 10px;">{{group.name}}</h4>
            <!-- {{ group | inspect }} -->
            <div class="directory_listPeople">
                <div class="row">
                    {% for item in group.people %}
                    <div class="col-md-4 col-sm-6 col-xs-6">
                        <a href="{{item.url}}">
                            <div ><img class="photo" src="{{item.image}}" ></div>
                            <div class="name" >{{item.name}}</div>
                        </a>
                        <div class="title">{{item.department}}</div>
                        <div class="title">{{item.title}}</div>
                        {% if item.buildingRoom != nil %}
                        <div class="buildingRoom">Office: {{item.buildingRoom}}</div>
                        {% endif %}
                        {% if item.phone != nil %}
                        <div class="phone">Phone: <a href="tel:{{item.phone}}">{{item.phone}}</a></div>
                        {% endif %}
                        <div class="email">Email: <a href="mailto:{{item.email}}">{{item.email}}</a></div>
                    </div>
                    {% endfor %}
                </div> 
            </div>  
        </div>
        {% endif %}
    {% endfor %}
</section>