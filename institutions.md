---
layout: default
title: Institutions
permalink: /institutions/
---
<section class="page-hero"><div class="shell narrow"><p class="eyebrow">Institutions</p><h1>A collaborative network across institutions and regions.</h1><p class="lead">Partner universities, research organisations, field stations and funders can be presented here.</p></div></section>
<section class="section"><div class="shell"><div class="institution-grid">{% for institution in site.data.institutions %}<article class="institution-card{% if institution.placeholder %} placeholder-card{% endif %}"><div class="logo-frame"><img src="{{ institution.logo | relative_url }}" alt="{% if institution.placeholder %}Institution logo placeholder{% else %}{{ institution.name }} logo{% endif %}"></div><div><p class="card-kicker">{{ institution.country }}</p><h2>{{ institution.name }}</h2><p>{{ institution.role }}</p>{% unless institution.website == '' %}<a class="arrow-link" href="{{ institution.website }}">Visit institution</a>{% endunless %}</div></article>{% endfor %}</div><div class="editor-note"><h2>Adding an institution</h2><p>Edit <code>_data/institutions.yml</code> and place its logo in <code>assets/images/institutions/</code>. Transparent PNG or SVG files work best.</p></div></div></section>
