---
layout: default
title: Accueil
---
<div class="post-grid">
  {% for post in site.posts %}
    <div class="post-card">
      <a href="{{ post.url | relative_url }}">

        {% if post.image %}
          <img src="{{ post.image | relative_url }}">
        {% else %}
          <img src="{{ '/assets/images/default.jpg' | relative_url }}">
        {% endif %}
        <h2>{{ post.title }}</h2>
      </a>
    </div>
{% endfor %}
</div>