---
layout: page
title: Clubs
---
<h2 align="center">
{% for team in site.teams %}
  <div class="team">
  <h3 align="center"><a href="{{ team.url }}"> <img src="{{team.thumb_image}}"> <br>{{ team.title }}</a>
  </h3>
  </div>
{% endfor %}
</h2>
