---
layout: page
title: Clubs
---
{% assign loopindex = 0 %}
{% for team in site.teams %}

  <div class="team1">{{ loopindex }} {{ rowfinder }}
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
 
{% endfor %}

