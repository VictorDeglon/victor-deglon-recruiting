---
layout: default
title: "Log | Victor Deglon"
description: "Dated updates after every tournament and PR for Victor Deglon, opposite hitter."
permalink: /log/
---

<section>
  <h1>Log</h1>
  <p class="lede">
    Updated after every tournament and every measurable PR. This is the
    freshness signal for the whole site — and the evidence trail behind
    the numbers on the <a href="{{ '/stats/' | relative_url }}">stats page</a>.
  </p>

  {% assign posts = site.posts %}
  {% if posts.size > 0 %}
  <div class="log-index">
    {% for post in posts %}
    <article class="log-index-item">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="meta"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time></p>
      <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    </article>
    {% endfor %}
  </div>
  {% else %}
  <p class="note">No entries yet — add a new file under <code>_posts/</code> after the next tournament or PR.</p>
  {% endif %}
</section>
