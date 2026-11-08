---
title: Software
lang: en
last_modified: 2026-11-08 01:45:30 UTC
layout: page
---

{% for sw in site.data.software -%}
- [{{ sw.name }}]({{ sw.url }}): {{ sw.description_en | default: sw.description | strip }}{% if sw.try_url %} ([Try it]({{ sw.try_url }})){% endif %}
{% endfor %}

Other personal projects are on [GitHub](https://github.com/yoriyuki). For work projects, see my [work page]({{ site.lab_url }}/en/).
