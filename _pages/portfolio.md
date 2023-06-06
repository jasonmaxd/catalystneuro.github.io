---
layout: splash
permalink: /portfolio/
title: "Portfolio"
author_profile: false
---

<style>
  .post-date {
  font-size:.625em;
  }
  .archive{
      @media (min-width: 80em){
          padding-right: 100px !important;
      }
  }
</style>

<h1>{{page.title}}</h1>

{% assign sorted = site.posts | reverse %}

{% for post in sorted %}

<br><span class="posts-date">{{ post.date | date_to_string }}</span>
<br><span class="posts-title"><a href="{{ post.url }}">{{ post.title }}</a></span>
<br><span class="posts-description">{% if post.excerpt %}{{ post.excerpt | markdownify | strip_html | truncate: 120 }}{% endif %}</span><br>
{% endfor %}