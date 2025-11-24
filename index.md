---
layout: default
title: seattle.cool
---

👉 <span class="new">New!</span> [Interview with SeattleNoise.org](/interviews/seattle-noise) (Nov 2025)

<table>
  <tbody>
  {% for item in site.data.resources %}
    <tr>
      <td><a href="{{ item.url }}">{{ item.name }}</a></td>
      <td><span class="arrow">→</span></td>
      <td><span class="category">{{ item.type }}</span></td>
      <td><span class="description">{{ item.description | markdownify | remove: '<p>' | remove: '</p>' }}</span></td>
      <td>{% if item.location %}<a href="{{ item.location }}" class="address-link">address</a>{% endif %}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
