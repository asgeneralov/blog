---
layout: default
title: "Blog"
---
{%- assign default_paths = site.pages | map: "path" -%}
{%- assign page_paths = site.header_pages | default: default_paths -%}
    <ul class="page-list">
        {%- for path in page_paths -%}
        {%- assign my_page = site.pages | where: "path", path | first -%}
        {%- if my_page.title and my_page.url != "/" -%}
        <li><a class="page-link" href="{{ my_page.url | relative_url }}">{{ my_page.title | escape }}</a></li>
        {%- endif -%}
        {%- endfor -%}
    </ul>

