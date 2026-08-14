---
layout: default
title: Store — Grilled Games
permalink: /store/
---

# Store

Our physical thumb drives are packed with our games — a retro collection you can hold in your hands. Each drive is a tribute to the cartridge days of gaming.

<div class="games-grid">
  {% for game in site.data.games %}
    <div class="game-card">
      <img src="{{ game.image | relative_url }}" alt="{{ game.title }}">
      <h3>{{ game.title }}</h3>
      <p>{{ game.description }}</p>
      <div class="buy-buttons">
        <a href="{{ game.stripe_url_physical }}" class="buy-button" target="_blank" rel="noopener">Physical Edition</a>
        <a href="{{ game.stripe_url_bundle }}" class="buy-button bundle" target="_blank" rel="noopener">Physical Edition + Steam Bundle</a>
        <a href="{{ game.stripe_url_steam }}" class="buy-button steam" target="_blank" rel="noopener">Steam</a>
      </div>
    </div>
  {% endfor %}
</div>

{% if site.data.games.size == 0 %}
<p>We're working on something exciting! Check back soon.</p>
{% endif %}
