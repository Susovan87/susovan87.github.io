---
layout: post
title: Daily notes
skip_related: true
---

I dump my daily notes here. It may not make sense to you, but seems very useful for others (including me).


<div id="notes">
  <ul>
    {% assign sorted = (site.notes | sort: 'date') | reverse %}
    {% for item in sorted %}
      <li><span>{{ item.date | date_to_string }} &raquo;</span><a href="{{ item.url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
</div> 
