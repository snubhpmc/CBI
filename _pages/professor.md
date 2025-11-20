---
layout: page
permalink: /professor/
title: PI
description: Principal investigator
years: [2024, 2023, 2022, 2021, 2020, 2019, 2017, 2016]
nav: false
nav_order: 4
---


{% assign pi = site.team | where: "role", "Principal Investigator" | sort: "order" %}
{% for member in pi %}
<div class="row" style="margin-bottom: 3rem;">
  <div class="col-sm-3">
    {% if member.photo %}
    <img src="{{ '/assets/img/team/' | append: member.photo | relative_url }}" class="img-fluid rounded-circle" alt="{{ member.name }}">
    {% endif %}
  </div>
  <div class="col-sm-9" style="display: flex; flex-direction: column;">
    <h4>{{ member.name }}</h4>
    <div><strong>{{ member.position }}</strong><br>
    {% if member.affiliation %}
      {% for line in member.affiliation %}
        {{ line }}<br>
      {% endfor %}
    {% endif %}
    </div>

    <div style="flex-grow: 1;">
      {{ member.content }}
    </div>

    <p style="display: flex; gap: 1rem; margin-bottom: 0;">
    {% if member.email %}
    <a href="#" onclick="navigator.clipboard.writeText('{{ member.email }}'); alert('Email copied to clipboard!'); return false;" title="Click to copy email address"><i class="fas fa-envelope"></i> Email</a>
    {% endif %}
    {% if member.google_scholar %}
    <a href="{{ member.google_scholar }}" target="_blank" title="Go to Google Scholar profile"><i class="ai ai-google-scholar"></i> Google Scholar</a>
    {% endif %}
    {% if member.homepage %}
    <a href="{{ member.homepage }}" target="_blank" title="Go to university homepage"><i class="fas fa-university"></i> Homepage</a>
    {% endif %}
    <a href="{{ '/teaching/' | relative_url }}" title="View teaching courses"><i class="fas fa-chalkboard-teacher"></i> Teaching</a>
    </p>
  </div>
</div>
{% endfor %}

---

## Teaching
<!-- Teaching -->

<div class="Teaching">

</div>

-----------------

## Professional Activities
<!-- Professional Activities  -->
-----------------


## Publications

-----------------