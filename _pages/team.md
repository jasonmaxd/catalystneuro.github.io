---
layout: splash
title: "Our Team"
permalink: /team/
collection: team
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/ourteam-header2034x444-1.jpg
---
<html>
{% assign sorted_members = site.team | sort: 'order' %}
{% assign total_members = sorted_members | size %}

{% for member in sorted_members %}
    {% include team_member.html member=member %}
    {% unless forloop.last %}
        <div style="border-bottom: 1px solid #5e616c; margin-bottom: 20px;"></div>
    {% endunless %}
{% endfor %}
</html>
