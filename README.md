---
layout: default
title: Home
---

<table>
  <tbody>
  {% for item in site.data.resources %}
    <tr>
      <td><a href="{{ item.url }}">{{ item.name }}</a></td>
      <td>{{ item.type }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>
