---
layout: page
title: ソフトウェア
lang : ja
last_modified: 
---


多分OCaml用のユニコード処理ライブラリ[Camomile](https://github.com/ocaml-community/Camomile)が一番使われています。

{% for sw in site.data.software -%}
- [{{ sw.name }}]({{ sw.url }}): {{ sw.description | strip }}
{% endfor %}

その他のリポジトリは[GitHub](https://github.com/yoriyuki)にあります。
