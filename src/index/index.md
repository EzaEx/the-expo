---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Home
permalink: "/a"
navpage: true
---

### Hey, I'm Tom. Here's my work

<script src="index/seamless.js" type="text/javascript" defer></script>

<canvas id="seamlessCanvas" width="50" height="50"></canvas>

[**_Seamless World_**](/about)

<br>
## Projects

{%- for page in site.pages -%}
{% if page.layout == "project" %}

-   **[{{ page.title }}]({{ page.url }})** {% if page.desc %} - {{ page.desc }} {% endif %}
    {% endif %}
    {% endfor %}
