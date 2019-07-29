---
layout: page
title: Apps
permalink: /apps/
---
{% for staff_member in site.staff_members %}
  <h2><a href="app1/technical/main.html">{{ staff_member.name }} - {{ staff_member.position }}</a></h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}

#Test