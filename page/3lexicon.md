---
layout: page
title: Lexicon
icon: th-list
type: page
---

{% for item in site.lexicon %}
  <div class="lexicon">
    <h2>{{ item.title }}</h2>
    {{ item.content }}
  </div>
{% endfor %}
