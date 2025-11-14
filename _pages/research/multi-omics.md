---
layout: page
title: "Multi-Omics Analysis"
permalink: /research/multi-omics/
description: "We utilize genomic data to develop personalized treatment strategies and improve patient outcomes through precision medicine approaches."
nav: false
---

<div style="margin-bottom: 2rem;">
  <p style="font-size: 0.9rem; color: #666;">
    <a href="{{ '/research/' | relative_url }}">← Back to Research</a>
  </p>
</div>

{% assign category = site.data.research | where: "category", "Multi-Omics Analysis" | first %}

<hr>

<h4 style="margin-top: 2rem; margin-bottom: 1.5rem;">Projects</h4>

{% for project in category.projects %}
<div style="padding: 2rem 0; {% if forloop.last == false %}border-bottom: 1px solid #e0e0e0;{% endif %}">
  <div class="row">
    {% if project.image and project.image != "" %}
    <div class="col-sm-4">
      <img src="{{ '/assets/img/research/' | append: project.image | relative_url }}"
           class="img-fluid rounded"
           alt="{{ project.title }}"
           style="max-height: 250px; object-fit: contain; width: 100%;">
    </div>
    <div class="col-sm-8">
    {% else %}
    <div class="col-sm-4">
      <div style="height: 250px; display: flex; align-items: flex-start; justify-content: center; padding-top: 1rem;">
        <span style="color: #999; font-size: 1rem; font-weight: 500;">Ongoing</span>
      </div>
    </div>
    <div class="col-sm-8">
    {% endif %}
      <h5 style="font-size: 1.3rem; font-weight: bold; color: #2c3e50;">
        {{ project.title }}
      </h5>
      <p style="margin-top: 1rem; color: #666;">{{ project.detail_description }}</p>

      {% if project.paper_title and project.paper_title != "" %}
      <p style="margin-top: 1rem; font-size: 0.9rem;">
        <i class="fas fa-file-alt"></i> <strong>Related Publication:</strong><br>
        {% if project.paper_link and project.paper_link != "" %}
        <a href="{{ project.paper_link }}" target="_blank" style="color: #007bff;">{{ project.paper_title }}</a>
        {% else %}
        {{ project.paper_title }}
        {% endif %}
      </p>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}
