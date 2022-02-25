---
title: Home
header: Tony Cavella
description: automation, infrastructure, security
permalink: /
layout: default
---
{% for post in site.posts %}
<div class="card w-100 shadow">
  <img class="card-img-top" src="{{ post.thumbnail }}" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">{{ post.title }}</h5>
    <p class="card-text">{{ post.excerpt }}</p>
    <small><a href="{{ post.url }}" class="card-link text-secondary">READ MORE</a></small>
  </div>
  <div class="card-footer bg-light d-flex bd-highlight">
    <div class="me-auto bd-highlight"><small class="text-muted">{{ post.date | date_to_string }}</small></div>
    <div class="bd-highlight"><small class="text-muted"><span class="badge bg-secondary">{{ post.category }}</span></small></div>
  </div>
</div>
<br>
{% endfor %}