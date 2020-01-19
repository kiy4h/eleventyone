---
title: Kiy4h
subtitle: A website I deployed to netlify using the EleventyOne template.
layout: layouts/base.njk
---

## My Posts

The pages found in in the posts

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>
