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
  .post-role{
    font-size: 1.1em;
  }

  .post-type {
    display: inline-block;
    font-size: 0.8em;
    font-weight: bold;
    padding: 2px 5px;
    border-radius: 4px;
    margin-right: 5px;
  }

  .blog-type {
    background-color: #ffa500;
    color: #fff;
  }

  .project-type {
    background-color: #008000;
    color: #fff;
  }

  .other-type {
    background-color: #808080;
    color: #fff;
  }
</style>

<h1>{{ page.title }}</h1>

{% assign sorted = site.posts | reverse %}

{% for post in sorted %}
  <div class="post">
    {% if post.type == 'blog' %}
      <span class="post-type blog-type">Blog</span>
    {% elsif post.type == 'project' %}
      <span class="post-type project-type">Project</span>
    {% else %}
      <span class="post-type other-type">Other</span>
    {% endif %}
    <span class="post-date">{{ post.date | date_to_string }}</span>
    <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
    {% if post.role %}
        <p class="post-role">Role: {{ post.role }}</p>
    {% endif %}
    <p class="post-description">{% if post.excerpt %}{{ post.excerpt | markdownify | strip_html | truncate: 120 }}{% endif %}</p>
  </div>
{% endfor %}