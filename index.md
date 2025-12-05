---
layout: default
title: Home
---

# Welcome to My Game Development Blog

Explore my latest games and 3D assets. Modern, mobile-friendly, and always up to date!

## Featured Games

{% for game in site.games %}
<div style="margin-bottom:2em;">
  <h2>{{ game.name }}</h2>
  <img src="{{ game.image }}" alt="{{ game.name }}" style="max-width:100%;height:auto;border-radius:10px;box-shadow:0 2px 8px #0002;">
  <p>{{ game.description }}</p>
  <a href="{{ game.link }}" target="_blank">Play / Store Page</a><br>
  <iframe width="320" height="180" src="{{ game.youtube | replace: 'watch?v=', 'embed/' }}" frameborder="0" allowfullscreen style="margin-top:0.5em;"></iframe>
</div>
{% endfor %}

[See all games &rarr;](/games)

## 3D Game Assets

{% for asset in site.assets %}
<div style="margin-bottom:2em;">
  <h2>{{ asset.name }}</h2>
  <img src="{{ asset.image }}" alt="{{ asset.name }}" style="max-width:100%;height:auto;border-radius:10px;box-shadow:0 2px 8px #0002;">
  <p>{{ asset.description }}</p>
  <a href="{{ asset.link }}" target="_blank">Download / Store Page</a><br>
  <iframe width="320" height="180" src="{{ asset.youtube | replace: 'watch?v=', 'embed/' }}" frameborder="0" allowfullscreen style="margin-top:0.5em;"></iframe>
</div>
{% endfor %}

[See all assets &rarr;](/assets)

---

Follow me on [GitHub]({{ site.social.github }}), [Twitter]({{ site.social.twitter }}), and [YouTube]({{ site.social.youtube }})!