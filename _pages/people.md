---
layout: page
permalink: /people/
title: People
description: Our lab members
nav: false
nav_order: 4
years: [2024, 2023, 2022, 2021, 2020, 2019, 2017, 2016]
---

#### Principal Investigator

{% for member in site.data.team_members.principal_investigator %}
<div class="row" style="margin-bottom: 3rem;">
  <div class="col-sm-3">
    {% if member.photo %}
    <img src="{{ '/assets/img/team/' | append: member.photo | relative_url }}" class="img-fluid rounded" alt="{{ member.name }}">
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
      {% if member.bio %}
      <p>{{ member.bio }}</p>
      {% endif %}
    </div>

    <p style="display: flex; gap: 1rem; margin-bottom: 0;">
    {% if member.email %}
    <a href="mailto:{{ member.email }}"><i class="fas fa-envelope"></i> Email</a>
    {% endif %}
    {% if member.google_scholar %}
    <a href="{{ member.google_scholar }}" target="_blank"><i class="ai ai-google-scholar"></i> Google Scholar</a>
    {% endif %}
    </p>
  </div>
</div>
{% endfor %}

---

#### Members

##### Current

<div class="row">
{% for student in site.data.team_members.phd_students %}
  <div class="col-sm-6 col-md-3" style="margin-bottom: 2rem;">
    <div style="display: flex; flex-direction: column; height: 100%;">
      {% if student.photo %}
      <img src="{{ '/assets/img/team/' | append: student.photo | relative_url }}" class="img-fluid rounded" alt="{{ student.name }}">
      {% endif %}
      <h5 style="margin-top: 0.8rem; font-size: 1rem;">{{ student.name }}</h5>
      <div style="flex-grow: 1;">
        <p style="font-size: 0.85rem;">
        <strong>{{ student.position }}</strong><br>
        {{ student.year }}<br>
        <em>{{ student.research }}</em>
        </p>
      </div>
      <p style="font-size: 0.85rem; display: flex; flex-direction: column; gap: 0.3rem; margin-top: 1rem; margin-bottom: 0;">
      {% if student.email %}
      <a href="mailto:{{ student.email }}"><i class="fas fa-envelope"></i> Email</a>
      {% endif %}
      {% if student.google_scholar %}
      <a href="{{ student.google_scholar }}" target="_blank"><i class="ai ai-google-scholar"></i> Google Scholar</a>
      {% endif %}
      </p>
    </div>
  </div>
{% endfor %}
</div>

---

##### Alumni

<div class="row">
{% for student in site.data.team_members.masters_students %}
  <div class="col-sm-6 col-md-3" style="margin-bottom: 2rem;">
    <div style="display: flex; flex-direction: column; height: 100%;">
      {% if student.photo %}
      <img src="{{ '/assets/img/team/' | append: student.photo | relative_url }}" class="img-fluid rounded" alt="{{ student.name }}">
      {% endif %}
      <h5 style="margin-top: 0.8rem; font-size: 1rem;">{{ student.name }}</h5>
      <div style="flex-grow: 1;">
        <p style="font-size: 0.85rem;">
        <strong>{{ student.position }}</strong><br>
        {{ student.year }}<br>
        <em>{{ student.research }}</em>
        </p>
      </div>
      <p style="font-size: 0.85rem; display: flex; flex-direction: column; gap: 0.3rem; margin-top: 1rem; margin-bottom: 0;">
      {% if student.email %}
      <a href="mailto:{{ student.email }}"><i class="fas fa-envelope"></i> Email</a>
      {% endif %}
      {% if student.google_scholar %}
      <a href="{{ student.google_scholar }}" target="_blank"><i class="ai ai-google-scholar"></i> Google Scholar</a>
      {% endif %}
      </p>
    </div>
  </div>
{% endfor %}
</div>

---

<div class="text-center" style="margin-top: 3rem; padding: 2rem; background-color: white; border-radius: 8px;">
  <h4>We're Hiring!</h4>
  <p style="font-size: 1.1rem; margin-top: 1rem;">
    We are actively seeking passionate students and researchers to join our team.<br>
    If you are interested in clinical bioinformatics and computational medicine,<br>
    don't hesitate to contact us!
  </p>
</div>
