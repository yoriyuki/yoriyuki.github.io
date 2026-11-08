---
title: Software
lang: en
last_modified:
layout: page
---

{% for sw in site.data.software -%}
- [{{ sw.name }}]({{ sw.url }}): {{ sw.description_en | default: sw.description | strip }}
{% endfor %}

Other personal projects are on [GitHub](https://github.com/yoriyuki). For work projects, see my [work page]({{ site.lab_url }}/en/).
