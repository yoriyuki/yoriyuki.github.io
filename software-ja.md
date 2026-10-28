---
layout: page
title: ソフトウェア
lang : ja
last_modified: 
---


多分OCaml用のユニコード処理ライブラリ[Camomile](https://github.com/ocaml-community/Camomile)が一番使われています。

{% assign repos = site.github.public_repositories | where_exp: "repo", "repo.fork == false" | sort: "stargazers_count" | reverse %}
{% for repo in repos limit: 5 -%}
- [{{ repo.name }}]({{ repo.html_url }}){% if repo.description %}: {{ repo.description }}{% endif %}
{% endfor %}

その他のリポジトリは[GitHub](https://github.com/yoriyuki)にあります。
