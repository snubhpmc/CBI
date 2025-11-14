---
layout: page
permalink: /teaching/
title: 
description: Materials for courses you taught. Replace this text with your description.
nav: false
nav_order: 3---

For now, this page is assumed to be a static description of your courses. You can convert it to a collection similar to `_projects/` so that you can have a dedicated page for each course.

Organize your courses by years, topics, or universities, however you like!


<div class="row" style="margin-top: 2rem;">
{% for area in site.data.research_areas limit:3 %}
  <div class="col-md-4" style="margin-bottom: 1.5rem;">
    {% if area.image %}
    <img src="{{ '/assets/img/research/' | append: area.image | relative_url }}" class="img-fluid rounded" alt="{{ area.title }}" style="margin-bottom: 1rem;">
    {% endif %}
    <h4>{{ area.icon }} {{ area.title }}</h4>
    <p style="font-size: 0.9em;">{{ area.description_ko | truncate: 100 }}</p>
    <a href="{{ '/research/' | relative_url }}">Learn more →</a>
  </div>
{% endfor %}
</div>