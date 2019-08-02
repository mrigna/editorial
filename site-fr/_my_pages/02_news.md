---
layout: post
title: News
permalink: /news/
index: true
---
<div class="module-content blog-list">
<h2>Dernières nouvelles</h2>
{% for post in site.posts offset: 0 limit: 5 %}
  <div class="post-teaser">
            <div class="submitted"><span class="blue">{{ post.date | date_to_string }}</span></div>
            {{ post.excerpt }} [...] <br />
            <div class="post-meta"><a class="read-more" href="{{ site.baseurl }}{{ post.url }}">Plus</a></div>
  </div>
  <hr class="rule-style1">
{% endfor %}
</div>