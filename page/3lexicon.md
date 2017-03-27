---
layout: page
title: Lexicon
permalink: /lexicon/
icon: th-list
type: page
---

* content
{:toc}


{% "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ".split("").each do |i| %}
 <h1>{{ i.chr }}</h1>
{% end %}

{% for item in site.lexicon %}
  <div class="lexicon">
    <a href="{{ item.url }}">{{ item.title }}</a>
  </div>
{% endfor %}
