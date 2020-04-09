---
layout: page
title: Clubs
---
{% for team in site.teams %}
  <div class="team">
  <h2><a href="{{ team.url }}"> <img src="{{team.feature_image}}"> <p align=justify <br>{{ team.title }}</p></a>
  </h2>
  </div>
{% endfor %}
