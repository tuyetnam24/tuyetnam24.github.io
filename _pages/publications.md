---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar or site.author.researchgate or site.author.orcid %}
  You can also find my articles on 
  {% if site.author.googlescholar %}<a href="{{ site.author.googlescholar }}">my Google Scholar</a>{% endif %}{% if site.author.researchgate %}, <a href="{{ site.author.researchgate }}">ResearchGate</a>{% endif %}{% if site.author.orcid %}, or <a href="{{ site.author.orcid }}">ORCID</a>{% endif %}.
{% else %}
  You can also find my articles on my <a href="https://scholar.google.com/">Google Scholar</a>, <a href="https://www.researchgate.net/">ResearchGate</a>, or <a href="https://orcid.org/">ORCID</a>.
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
