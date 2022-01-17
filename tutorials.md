---
layout: page
permalink: /tutorials/
title: Tutorials
description: Brief (or lengthy) jupyter notebooks to explain concepts and enable insight.
---

<ul class="post-list">
{% for tutorial in site.tutorials reversed %}
    <li>
        <h3><a class="tutorial-title" href="{{ tutorial.url | prepend: site.baseurl }}">{{ tutorial.title }}</a></h3>
        <p class="post-meta">{{ tutorial.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>