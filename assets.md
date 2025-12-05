---
layout: default
title: 3D Assets
permalink: /assets/
---

# 3D Game Assets

A collection of my 3D models and asset packs for game development.

{% for asset in site.assets %}
<div style="margin-bottom:2em;">
  <h2>{{ asset.name }}</h2>
  <img src="{{ asset.image }}" alt="{{ asset.name }}" style="max-width:100%;height:auto;border-radius:10px;box-shadow:0 2px 8px #0002;">
  <p>{{ asset.description }}</p>
  <a href="{{ asset.link }}" target="_blank">Download / Store Page</a><br>
  <iframe width="320" height="180" src="{{ asset.youtube | replace: 'watch?v=', 'embed/' }}" frameborder="0" allowfullscreen style="margin-top:0.5em;"></iframe>
</div>
{% endfor %}
