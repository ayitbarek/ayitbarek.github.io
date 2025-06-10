---
layout: default
title: "Publications2"
permalink: /publications2/
---

## Publications

<ul class="pub-list">
  {% assign pubs = site.data.publications2 %}
  {% for pub in pubs %}
    <li>
      <strong>{{ pub.authors }}</strong> ({{ pub.year }}).<br>
      <em>{{ pub.title }}</em>.<br>
      {% if pub.journal %}
        {{ pub.journal }}, <strong>{{ pub.volume }}</strong>({{ pub.issue }}), {{ pub.pages }}.<br>
      {% endif %}
      {% if pub.patent_office %}
        Patent {{ pub.patent_office }} - {{ pub.patent_number }} ({{ pub.publication_date }})<br>
      {% endif %}
      {% if pub.doi != '' %}
        <a href="{{ pub.doi }}" target="_blank">{{ pub.doi }}</a>
      {% endif %}
    </li>
  {% endfor %}
</ul>

