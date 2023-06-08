---
layout: splash
permalink: /portfolio/
title: "Portfolio"
author_profile: false
---

<style>
  .post-date {
    font-size: 0.8em;
    color: #999;
  }

  .post-title {
    font-size: 1.2em;
    margin: 5px 0;
  }

  .post-description {
    margin-bottom: 10px;
  }

  .post-tags {
    font-size: 0.8em;
    color: #666;
  }
</style>

<h1>{{ page.title }}</h1>

{% assign sorted = site.posts | reverse %}

{% for post in sorted %}
  <div class="post">
    <span class="post-date">{{ post.date | date_to_string }}</span>
    <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-description">{% if post.excerpt %}{{ post.excerpt | markdownify | strip_html | truncate: 120 }}{% endif %}</p>
    <p class="post-tags">{% if post.tags %}Tags: {% for tag in post.tags %}<span class="tag">{{ tag }}</span> {% endfor %}{% endif %}</p>
  </div>
{% endfor %}