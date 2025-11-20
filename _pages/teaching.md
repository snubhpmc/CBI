---
layout: page
permalink: /teaching/
title: Teaching
description: Courses and teaching materials
nav: false
nav_order: 3
---


**Precision Medicine and Healthcare (M3384.000800)** 
Precision medicine and healthcare are key elements of future medicine through the accumulation of medical information and the use of artificial intelligence. This course intends to give an overview of the various aspects of precision medicine and healthcare. The course will deal with genomics, medical images, artificial intelligence, and digital healthcare, providing a deeper understanding of precision medicine for students planning to pursue healthcare convergence studies.



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