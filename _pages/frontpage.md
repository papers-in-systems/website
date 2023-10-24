---
permalink: /
layout: page
# title: ""
list_title: My blog posts
---

Upcoming
{% assign session = site.sessions.last %}

  <article class="session-excerpt">
    <a href="{{session.url}}">
    <div>
    {{session.date | date: site.minima.date_format }}
    {%- if session.presenter -%} {% for presenter in session.presenter %}
        <span itemprop="performer" itemscope itemtype="http://schema.org/Person">
          <span class="p-performer h-card" itemprop="name"
            >{{ presenter.name }}
          </span>
        </span>
        {% endfor %}
        {%- endif -%}

      <div class="title">{{ session.title }}</div>
      {{ session.slug }}
    </div>
    </a>
  </article>