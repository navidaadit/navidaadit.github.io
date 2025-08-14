---
permalink: /publications/
title: "Publications"
layout: single
author_profile: true
---

{% assign pubs = site.publications | sort: "date" | reverse %}
{% if pubs and pubs.size > 0 %}
<ul>
{% for p in pubs %}
  <li>
    <strong>{{ p.title }}</strong>.
    <em>{{ p.venue }}</em>,
    {{ p.date | date: "%Y" }}.
    {% if p.citation %} {{ p.citation }}{% endif %}
    {% if p.paperurl %} <a href="{{ p.paperurl }}">link</a>{% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
<p>No items found in <code>_publications/</code>. Make sure the files are there and start with YAML front matter.</p>
{% endif %}
