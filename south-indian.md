---
layout: default
title: South Indian Movies
permalink: /south-indian/
---

<div class="sec-head">🎬 South Indian Movies</div>

{% for post in site.posts %}
  {% if post.categories contains 'South' %}
    <a href="{{ site.baseurl }}{{ post.url }}" class="movie-card">
        <img src="{{ post.image }}" class="mc-img" alt="poster" loading="lazy">
        <div class="mc-info">
            <h3 class="mc-title">{{ post.title }}</h3>
            <div class="tag-row">
                <span class="tag t-blue">{{ post.quality }}</span>
                <span class="tag t-gray">{{ post.year }}</span>
            </div>
        </div>
    </a>
  {% endif %}
{% endfor %}

<div class="sec-head">📁 Other Categories</div>
<div class="cat-grid">
    <a href="/" class="cat-btn">← Home</a>
    <a href="/bollywood/" class="cat-btn">Bollywood →</a>
</div>


