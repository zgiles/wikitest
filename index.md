---
layout: default
title: WikiTest Main Page
---

# Wiki Test

This is a Wiki Test that has some links.  
* For example a Link to [New Page](hardware/newpage)

{% for p in site.pages %}
  {{ p.category }}
{% endfor %}

{% assign catpages = site.pages | group_by:"category" %}
{% for p in catpages %}
  {{ p }}
{% endfor %}
