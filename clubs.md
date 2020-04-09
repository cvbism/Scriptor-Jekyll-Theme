---
layout: page
title: Clubs
---
{% assign loopindex = 0 %}
{% for team in site.teams %}
{% assign loopindex = loopindex | plus: 1 %}
{% assign rowfinder = loopindex | modulo: 4 %}
 
 {% if rowfinder == 1 %}
      
  <div class="row">
  <div class="team1">{{ loopindex }} {{ rowfinder }}
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
  
  {% elsif rowfinder == 0 %}
  
  <div class="team1">{{ loopindex }} {{ rowfinder }}
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
  
   {% else %}
   <div class="team1">{{ loopindex }} {{ rowfinder }}
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
  
   {% endif %}
  {% endif %}
  
  
{% endfor %}
{% if rowfinder != 0 %}
      </div>
{% endif %}
