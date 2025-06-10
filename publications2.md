---
layout: default
title: "publication2"
permalink: /publications2/
---

## Publications

<ul class="pub-list">
  {% assign pubs = site.data.publications %}
  {% for pub in pubs %}
    <li>
      <strong>{{ pub.authors }}</strong> ({{ pub.year }}).<br>
      <em>{{ pub.title }}</em>.<br>
      {{ pub.journal }}, <strong>{{ pub.volume }}</strong>({{ pub.issue }}), {{ pub.pages }}.<br>
      <a href="{{ pub.doi }}" target="_blank">{{ pub.doi }}</a>
    </li>
  {% endfor %}
</ul>

