---
title: Home
header: Tony Cavella
description: automation, infrastructure, security
permalink: /
layout: default
---
<p class="tldr">Hey, my name is Tony! I'm a Linux nerd, mobile infrastructure engineer, and general tech enthusiast! This is my personal blog, somewhere to share my personal thoughts and projects. There is no gaurentee that I will update this blog with any regularity, but will try my best to post content I find interesting.</p>

<h3>Blog Posts</h3>
<div class="card" style="width: 18rem;">
  <img class="card-img-top" src="..." alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
  <div class="card-body">
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>

{% for post in site.posts %}
<div class="card mb-3">
  <img class="card-img-top" src="..." alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">{{ post.title }}</h5>
    <p class="card-text">{{ post.description }}</p>
    <p class="card-text"><small class="text-muted"><a href="{{ post.url}}">Read More...</a></small></p>
    <p class="card-text"><small class="text-muted">{{ post.date | date_to_string }}</small></p>
  </div>
</div>
{% endfor %}