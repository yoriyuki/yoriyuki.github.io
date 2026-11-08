---
layout: page
title: ソフトウェア
lang : ja
last_modified: 
---


多分OCaml用のユニコード処理ライブラリ[Camomile](https://github.com/ocaml-community/Camomile)が一番使われています。

{% for sw in site.data.software -%}
- [{{ sw.name }}]({{ sw.url }}): {{ sw.description | strip }}{% if sw.try_url %}（[ブラウザで試す]({{ sw.try_url }})）{% endif %}
{% endfor %}

その他の個人プロジェクトは[GitHub](https://github.com/yoriyuki)にあります。仕事で作っているものは[仕事用のページ]({{ site.lab_url }})をご覧ください。
