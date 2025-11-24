---
layout: default
title: seattle.cool
---

<div class="announce">👉 <span class="new">New!</span> <a href="{{ '/interviews/seattle-noise' | relative_url }}">Interview with SeattleNoise.org</a> (Nov 2025)</div>

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
