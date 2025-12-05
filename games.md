---
layout: default
title: Games
permalink: /games/
---

# My Games

A showcase of my released and in-development games.

{% for game in site.games %}
<div style="margin-bottom:2em;">
  <h2>{{ game.name }}</h2>
  <img src="{{ game.image }}" alt="{{ game.name }}" style="max-width:100%;height:auto;border-radius:10px;box-shadow:0 2px 8px #0002;">
  <p>{{ game.description }}</p>
  <a href="{{ game.link }}" target="_blank">Play / Store Page</a><br>
  <iframe width="320" height="180" src="{{ game.youtube | replace: 'watch?v=', 'embed/' }}" frameborder="0" allowfullscreen style="margin-top:0.5em;"></iframe>
</div>
{% endfor %}
