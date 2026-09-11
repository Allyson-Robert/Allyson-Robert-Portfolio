---
layout: page
title: Project pages
permalink: /projects/
nav: false
---

[Research project landing page goes here. Each project below is generated from a markdown file in `_projects`.]

{% assign sorted_projects = site.projects | sort: 'importance' %}
{% for project in sorted_projects %}
- [{{ project.title }}]({{ project.url | relative_url }}) — {{ project.description }}
{% endfor %}
