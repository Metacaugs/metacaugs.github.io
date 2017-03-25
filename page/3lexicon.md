---
layout: page
title: Lexicon
permalink: /lexicon/
icon: th-list
type: page
---

* content
{:toc}

{% for char in 0..5 %}
<div class="letter">
{{ char }}
</div>
{% endfor %}

{% for item in site.lexicon %}
  <div class="lexicon">
    <a href="{{ item.url }}">{{ item.title }}</a>
  </div>
{% endfor %}
