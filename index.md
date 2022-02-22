---
title: Home
header: Tony Cavella
description: automation, infrastructure, security
permalink: /
layout: default
---
{% for post in site.posts %}
<div class="card w-100 shadow">
  <img class="card-img-top" src="/assets/images/placeholder.svg" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">{{ post.title }}</h5>
    <p class="card-text">{{ post.excerpt }}</p>
    <a href="{{ post.url }}" class="card-link">READ MORE</a>
  </div>
  <div class="card-footer bg-light">
    <small class="text-muted">{{ post.date | date_to_string }}</small>
  </div>
</div>
<br>
{% endfor %}