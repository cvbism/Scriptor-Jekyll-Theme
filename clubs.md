---
layout: page
title: Clubs
---
<div class="clubs" align="justify">
{% for team in site.teams %}
  
  <div class="team1">
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
  
  <div class="team2">
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
 
  
{% endfor %}
</div>
