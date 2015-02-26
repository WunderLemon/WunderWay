---
layout: section
title: Working With Us
---

text text text

{% comment %}
  The code below dynamically generates a list of pages with
  section = how in the front-matter.
{% endcomment %}

{% assign pages_list = site.pages %}
{% for node in pages_list %}
  {% if node.title != null %}
    {% if node.section == "workwithus" and node.subsection == null %}
<a class="section-list" href="{{ node.url }}">{{ node.title }}</a>
    {% endif %}
  {% endif %}
{% endfor %}