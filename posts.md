---
layout: page
permalink: /posts/
title: Posts
description: Blogs relevant to neuroscience, neurotechnology and machine learning in healthcare.
---

<ul class="post-list">
{% for post in site.posts reversed %}
    <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>