---
layout: page
title: Lexicon
permalink: /lexicon/
icon: th-list
type: page
---

* content
{:toc}


{% for i in (1..10) %}
<span class="lexicon">
    ## <h2>{{ i }}</h2>
</span>
{% endfor %}

{% for item in site.lexicon %}
  <div class="lexicon">
    <a href="{{ item.url }}">{{ item.title }}</a>
  </div>
{% endfor %}
