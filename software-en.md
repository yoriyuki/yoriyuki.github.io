---
title: Software
lang: en
layout: page
---

{% for sw in site.data.software -%}
- [{{ sw.name }}]({{ sw.url }}): {{ sw.description_en | default: sw.description | strip }}{% if sw.try_url %} ([Try it]({{ sw.try_url }})){% endif %}
{% endfor %}

Other personal projects are on [GitHub](https://github.com/yoriyuki). For work projects, see my [work page]({{ site.lab_url }}/en/).
