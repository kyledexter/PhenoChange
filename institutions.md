---
layout: default
title: Institutions
permalink: /institutions/
---
<section class="page-hero"><div class="shell"><p class="eyebrow">Partners</p><h1>Institutions</h1></div></section>
<section class="section"><div class="shell"><div class="institution-grid equal-institutions">{% for institution in site.data.institutions %}<article class="institution-card"><div class="logo-frame"><img src="{{ institution.logo | relative_url }}" alt="{{ institution.name }} logo"></div><div><h2>{{ institution.name }}</h2><p>{{ institution.country }}</p><a class="arrow-link" href="{{ institution.website }}" target="_blank" rel="noopener">Visit website →</a></div></article>{% endfor %}</div></div></section>
