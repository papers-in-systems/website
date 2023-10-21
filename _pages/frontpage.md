---
permalink: /
layout: page
# title: ""
list_title: My blog posts
---

Upcoming
{% assign session = site.sessions.last %}

<article class="session-excerpt"><a href="{{session.url}}">
  <div>
{{session.date | date: site.minima.date_format }} &middot; {{ session.presenter }}</div>
  <div class="title">{{ session.title }}</div>
{{ session.content | strip_html | truncatewords: 15 }}
</a>
</article>
