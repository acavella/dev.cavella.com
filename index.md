---
title: Home
header: Tony Cavella
description: automation, infrastructure, security
permalink: /
layout: default
---
<p class="tldr">Hey, my name is Tony! I'm a Linux nerd, mobile infrastructure engineer, and general tech enthusiast! This is my personal blog, somewhere to share my personal thoughts and projects. There is no gaurentee that I will update this blog with any regularity, but will try my best to post content I find interesting.</p>

<h3>Blog Posts</h3>

{% for post in site.posts %}
<div class="card col-md-8">
  <img class="card-img-top" src="/assets/images/placeholder.svg" alt="Card image cap">
  <div class="card-body">
    <h5 class="card-title">{{ post.title }}</h5>
    <p class="card-text">{{ post.description }}</p>
    <p class="card-text"><small class="text-muted"><a href="{{ post.url}}">Read More...</a></small></p>
    <p class="card-text"><small class="text-muted">{{ post.date | date_to_string }}</small></p>
  </div>
</div>
</br>
{% endfor %}