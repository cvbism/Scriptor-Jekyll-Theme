---
layout: default
title: Clubs
---
{% for team in site.teams %}
  <div class="team">
  <h2 align="center"><a href="{{ team.url }}"> <img src="{{team.feature_image}}"> <br>{{ team.title }}</a>
  </h2>
  </div>
{% endfor %}
