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

{% for i in (a..f) %}
    ## {{ i }}
{% endfor %}

{% for item in site.lexicon %}
  <div class="lexicon">
    <a href="{{ item.url }}">{{ item.title }}</a>
  </div>
{% endfor %}
