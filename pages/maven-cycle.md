---
title: Цикл статей об Инструменте Maven
layout: default
---
# Цикл статей о инструменте Maven
<ol class="page-list">
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
