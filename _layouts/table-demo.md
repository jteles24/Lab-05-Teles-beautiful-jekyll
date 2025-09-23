---
layout: liquid-table
title: amiright?
permalink: /table-demo/
reynolds:
  strengths: [good father, funny, dated alanis morissette]
  weaknesses: [singing, green lantern movie, tennis backhand]
gosling:
  strengths: [builds houses, is a real boy, never dated alanis morissette]
  weaknesses: [micky mouse club, cries a lot, not ryan reynolds]
---

![](img/ryan-v-ryan.jpg)

{% assign r = page.reynolds %}
{% assign g = page.gosling %}

<table>
  <tr><th>Attribute</th><th>Ryan Reynolds</th><th>Ryan Gosling</th></tr>
  <tr>
    <td>Strengths</td>
    <td><ul>{% for s in r.strengths %}<li>{{ s }}</li>{% endfor %}</ul></td>
    <td><ul>{% for s in g.strengths %}<li>{{ s }}</li>{% endfor %}</ul></td>
  </tr>
  <tr>
    <td>Weaknesses</td>
    <td><ul>{% for w in r.weaknesses %}<li>{{ w }}</li>{% endfor %}</ul></td>
    <td><ul>{% for w in g.weaknesses %}<li>{{ w }}</li>{% endfor %}</ul></td>
  </tr>
</table>
