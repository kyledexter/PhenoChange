---
layout: default
title: Publications
permalink: /publications/
---
<section class="page-hero"><div class="shell narrow"><p class="eyebrow">Publications</p><h1>Research emerging from PhenoChange and its collaborations.</h1><p class="lead">Peer-reviewed work using phenocameras and related approaches in tropical dry forests and savannas.</p></div></section>
<section class="section"><div class="shell publication-list">{% assign publications = site.data.publications | sort: 'year' | reverse %}{% for publication in publications %}<article class="publication"><div class="publication-year">{{ publication.year }}</div><div><h2><a href="{{ publication.url }}">{{ publication.title }}</a></h2><p class="publication-authors">{{ publication.authors }}</p><p><em>{{ publication.journal }}</em> {{ publication.volume }}{% if publication.issue %}({{ publication.issue }}){% endif %}{% if publication.article %}, {{ publication.article }}{% endif %}.</p><div class="publication-meta"><a href="{{ publication.url }}">DOI: {{ publication.doi }}</a>{% if publication.open_access %}<span>Open access</span>{% endif %}</div></div></article>{% endfor %}<div class="editor-note"><h2>Adding a publication</h2><p>Add a new record to <code>_data/publications.yml</code>. Publications are automatically ordered by year.</p></div></div></section>
