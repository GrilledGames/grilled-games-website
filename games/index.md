---
layout: default
title: Our Games — Grilled Games
permalink: /games/
---

# Our Games

<div class="games-grid">
  {% for game in site.data.games %}
    <div class="game-card">
      <img src="{{ game.image | relative_url }}" alt="{{ game.title }}">
      <h3>{{ game.title }}</h3>
      <p>{{ game.description }}</p>
      <div class="buy-buttons">
        <a href="{{ game.stripe_url_physical }}" class="buy-button" target="_blank" rel="noopener">Physical Edition</a>
        <a href="{{ game.stripe_url_steam }}" class="buy-button" target="_blank" rel="noopener">Steam</a>
      </div>
    </div>
  {% endfor %}
</div>

{% if site.data.games.size == 0 %}
<p>We're working on something exciting! Check back soon.</p>
{% endif %}
