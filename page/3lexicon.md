---
layout: page
title: Lexicon
permalink: /lexicon/
icon: th-list
type: page
---

* content
{:toc}

# Header
## Header 2

{% for i in (1..10) %}
    ## {{ i.chr }}
{% endfor %}

{% for item in site.lexicon %}
  <div class="lexicon">
    <a href="{{ item.url }}">{{ item.title }}</a>
  </div>
{% endfor %}
