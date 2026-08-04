---
layout: default
title: People
permalink: /people/
---
<section class="page-hero"><div class="shell"><p class="eyebrow">The network</p><h1>People</h1></div></section>
{% assign groups = "Coordinators,Site Leaders" | split: "," %}
{% for group in groups %}
<section class="section {% if group == 'Site Leaders' %}muted-section{% endif %}">
  <div class="shell">
    <div class="people-section-heading"><h2>{{ group }}</h2></div>
    <div class="card-grid people-grid {% if group == 'Coordinators' %}coordinator-grid{% else %}site-leader-grid{% endif %}">
    {% for person in site.data.people %}{% if person.group == group %}
      <article class="person-card">
        <div class="person-photo-wrap"><img src="{{ person.image | relative_url }}" alt="Portrait of {{ person.name }}" loading="lazy"></div>
        <div class="card-body">
          <h3>{{ person.name }}</h3>
          <p class="institution-name">{{ person.institution }}</p>
          <a class="button button-secondary profile-button" href="{{ person.website }}" target="_blank" rel="noopener">{{ person.link_label }}</a>
        </div>
      </article>
    {% endif %}{% endfor %}
    </div>
  </div>
</section>
{% endfor %}
