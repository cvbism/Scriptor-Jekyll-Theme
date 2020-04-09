---
layout: teams
title: Clubs
---
{% for team in site.teams %}
  <div class="team">
  <h2><img src="{{team.feature_image}}" href="{{ team.url }}">{{ team.title }}</a></h2>
  </div>
{% endfor %}
