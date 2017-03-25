---
layout: page
title: Lexicon
permalink: /lexicon/
icon: th-list
type: page
---

* content
{:toc}
{% for char in [*('0'..'9'),*('a'..'z')] %}
<div class="letter">
{{char}}
</div>
{% endfor %}

{% for item in site.lexicon %}
  <div class="lexicon">
    <h1><a href="{{ item.url }}">{{ item.title }}</a></h1>
  </div>
{% endfor %}
