---
title: Software
lang: en
last_modified:
layout: page
---

{% assign repos = site.github.public_repositories | where_exp: "repo", "repo.fork == false" | sort: "stargazers_count" | reverse %}
{% for repo in repos limit: 5 -%}
- [{{ repo.name }}]({{ repo.html_url }}){% if repo.description %}: {{ repo.description }}{% endif %}
{% endfor %}

Other repositories are on [GitHub](https://github.com/yoriyuki).
