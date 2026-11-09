---
title: ISO 27001 Series
icon: fas fa-shield-alt
order: 0
---

Implementing ISO/IEC 27001:2022 step by step, following the fictitious company **MK Consults** from zero to certification-ready. New to the series? Start at the top and read in order.

{% assign series = site.categories.ISO27001 | sort: "date" %}
{% for post in series %}
<div class="mb-4">
  <h3 class="mt-0 mb-1" style="font-size:1.15rem;">
    <span class="text-muted me-2">{{ forloop.index }}.</span><a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h3>
  <div class="text-muted small">{{ post.date | date: "%b %-d, %Y" }}</div>
</div>
{% endfor %}

*MK Consults is a fictitious company. All names, figures and documents in this series are illustrative and created for educational purposes.*
