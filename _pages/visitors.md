---
layout: page
permalink: /visitors/
title: visitors
description: a list of international visitors to the lab
nav: true
nav_order: 8
---

<table class="table table-sm">
  <colgroup>
    <col span="1" style="width: 60px;">
    <col span="1" style="width: 180px;">
    <col span="1" style="width: 160px;">
    <col span="1" style="width: 220px;">
    <col span="1" style="width: 80px;">
  </colgroup>

  <tr>
    <th>Year</th>
    <th>Name</th>
    <th>Position</th>
    <th>Institution</th>
    <th>Country</th>
  </tr>

  {% for visitor in site.data.visitors %}
  <tr>
    <td>{{ visitor.year }}</td>
    <td>{{ visitor.name }}</td>
    <td>{{ visitor.position }}</td>
    <td>{{ visitor.institution }}</td>
    <td>{{ visitor.country }}</td>
  </tr>
  {% endfor %}

</table>
