---
layout: page
permalink: /people/professor/
title: Professor
description: Principal investigator
years: [2024, 2023, 2022, 2021, 2020, 2019, 2017, 2016]
nav: false
---


{% for member in site.data.team_members.principal_investigator %}
<div class="row" style="margin-bottom: 3rem;">
  <div class="col-sm-3">
    {% if member.photo %}
    <img src="{{ '/assets/img/team/' | append: member.photo | relative_url }}" class="img-fluid rounded" alt="{{ member.name }}">
    {% endif %}
  </div>
  <div class="col-sm-9">
    <h4>{{ member.name }}</h4>
    <div><strong>{{ member.position }}</strong><br>
    {% if member.affiliation %}
      {% for line in member.affiliation %}
        {{ line }}<br>
      {% endfor %}
    {% endif %}
    </div>

    {% if member.bio %}
    <p>{{ member.bio }}</p>
    {% endif %}

    <p>
    {% if member.email %}
    <a href="mailto:{{ member.email }}"><i class="fas fa-envelope"></i> Email</a> &nbsp;
    {% endif %}
    {% if member.google_scholar %}
    <a href="{{ member.google_scholar }}" target="_blank"><i class="ai ai-google-scholar"></i> Google Scholar</a>
    {% endif %}
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
## Publication

<!-- Publications -->
<div class="publications">

{% for y in page.years %}

  <h2 class="year">{{ y }}</h2>

  {% bibliography -f papers -q @*[year={{y}}] %}

{% endfor %}

</div>
