---
layout: page
title: Clubs
---
<div class="clubs" align="justify">
{% for team in site.teams %}
{% assign mod = forloop.index | modulo: 4 %}
{{ mod }}:{{team.title}}
{% if mod == 1 %}
  <div class="team1">
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
  {% elsif mod == 2 %}
  <div class="team2">
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
  
  <hr>
{% endif %}
  
{% endfor %}
</div>
