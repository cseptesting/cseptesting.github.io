---
layout: page
title: People
permalink: /people/
---

CSEP is an international collaboration of earth scientists that share a common goal of understanding the predictability of earthquakes. The CSEP community works together to devise prospective earthquake forecasting experiments to assess hypotheses about natural earthquake processes. The following people have an active role in current CSEP activities:

<div class="people-list">
  {% for person in site.data.people %}
    <div class="person-card" style="display: flex; align-items: center; margin-bottom: 2rem;">
      <img src="{{ person.image | relative_url }}" alt="{{ person.name }}" style="width: 100px; height: 100px; object-fit: cover; border-radius: 50%; margin-right: 1.5rem;" />
      <div>
        <h3 style="margin: 0 0 0.25rem 0;">{{ person.name }}</h3>
        <p style="margin: 0 0 0.5rem 0; font-style: italic; color: #555;">{{ person.role }}</p>
        <p style="margin: 0;">{{ person.contact }}</p>
      </div>
    </div>
  {% endfor %}
</div>
