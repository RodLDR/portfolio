---
layout: default
title: Home
---

# Rodrigo LDR — Mechatronics Engineer

TODO: one-paragraph intro — background, focus areas (robotics, embedded systems, CAD), what you're looking for.

## Projects

<ul class="project-list">
{% assign projects = site.projects | sort: 'date' | reverse %}
{% for project in projects %}
  <li>
    <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    <p>{{ project.summary }}</p>
  </li>
{% endfor %}
</ul>
