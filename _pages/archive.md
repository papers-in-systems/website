---
permalink: /sessions
layout: page
title: Past sessions
---

<ul class="session-list">
  {% for session in site.sessions reversed %}
    <li class="session" data-timestamp="{{ session.date | date: '%s%L'}}">
      <a href="{{ session.url }}">
        <div>
        {{session.date | date: '%B %Y'}} &middot; {{ session.presenter }}</div>
        <div class="title">{{ session.title }}</div>
      </a>
    </li>

{% endfor %}

    <script>
      Array.from(document.querySelectorAll('.session')).forEach(session => {
        if (parseInt(session.dataset.timestamp) > Date.now()) {
          session.classList.add('hidden')
        }
      })
    </script>

</ul>
<p>This archive is a work in progress - we're working to add our past sessions for posterity.</p>
