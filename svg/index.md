---
layout: default
title: SVG
---

#SVG
Collection of SVG examples.

<ul>
{% for example in site.data.examples.svg.examples %}
  <li>
    <a href="{{ site.path }}/svg/{{ example.folder}}">
      {{ example.title }}
    </a>
  </li>
{% endfor %}
</ul>