---
layout: default
title: "Blog"
---

# Blog

## Цикл статей о инструменте Maven
<ol>
{% for maven_member in site.maven %}
  <!-- <h2>{{ maven_member.title }}</h2> -->
  <li>
  <a href="{{ maven_member.url }}">
    {{ maven_member.title }}
  </a>
  </li>
  <!-- <p>{{ maven_member.content | markdownify }}</p> -->
{% endfor %}
</ol>
