---
layout: liquid-table
title: amiright?
permalink: /table-demo/
reynolds:
  strengths:
    - good father
    - funny
    - dated alanis morissette
  weaknesses:
    - singing
    - green lantern movie
    - tennis backhand
gosling:
  strengths:
    - builds houses
    - is a real boy
    - never dated alanis morissette
  weaknesses:
    - micky mouse club
    - cries a lot
    - not ryan reynolds
---

![Ryan vs Ryan](/assets/ryan-v-ryan-Lab5.jpg)

{% assign r = page.reynolds %}
{% assign g = page.gosling %}

<table>
  <thead>
    <tr>
      <th>Attribute</th>
      <th>Ryan Reynolds</th>
      <th>Ryan Gosling</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Strengths</td>
      <td><ul>{% for s in r.strengths %}<li>{{ s }}</li>{% endfor %}</ul></td>
      <td><ul>{% for s in g.strengths %}<li>{{ s }}</li>{% endfor
