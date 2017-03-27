---
layout: page
title: "Lexicon"
permalink: /lexicon/
icon: th-list
type: page
---

* content
{:toc}

{% for item in "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ" | split:"" %}
  {{ item }}
{% endfor %}


{% for item in site.lexicon %}
  <div class="lexicon">
  <h2><a href="{{ item.url }}">{{ item.title }}</a></h2>
</div>
{% endfor %}
