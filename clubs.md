---
layout: page
title: Clubs
---
<h2 align="center">
{% for team in site.teams %}

  <div class="team" style="padding: 40px; display: inline-block;">
    <h3 align="center">
      <a href="{{ team.url }}"> 
        <img src="{{team.thumb_image}}"> 
        <br>{{ team.title }}
        <p><sub>{{team.description}}</sub></p>
      </a>
    </h3>
  </div>
 
{% endfor %}
</h2>
