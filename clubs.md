---
layout: page
title: Clubs
---
{% for teams in site.teams %}
  <div class="teams">
    <h2><a href="{{ teams.url }}">{{ teams.title }}</a></h2>
  </div>
{% endfor %}
