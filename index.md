---
layout: default
title: "Victor Deglon | Opposite Hitter Volleyball Recruiting Profile"
description: "Volleyball recruiting profile for Victor Deglon, opposite hitter. Measurables, film, schedule, and academics."
permalink: /
---

<section class="hero">
  <div class="hero-grid">
    <div class="hero-main">
      <h1>{{ site.data.profile.name }}</h1>
      <p class="lede">
        {{ site.data.profile.position }} &middot; Class of {{ site.data.profile.class_year | default: "TBD" }}
        {% if site.data.profile.club_team != "" %} &middot; {{ site.data.profile.club_team }}{% endif %}
      </p>

      {% assign reach = site.data.stats | where: "metric", "Approach / Touch Reach" | first %}
      {% assign serve = site.data.stats | where: "metric", "Serve Speed" | first %}
      <ul class="facts">
        <li><strong>Height:</strong> {{ site.data.profile.height | default: "TBD" }}</li>
        {% if reach %}<li><strong>Approach Reach:</strong> {{ reach.current }}</li>{% endif %}
        {% if serve %}<li><strong>Serve:</strong> {{ serve.current }}</li>{% endif %}
        {% if site.data.profile.club_division != "" %}<li><strong>Division:</strong> {{ site.data.profile.club_division }}</li>{% endif %}
      </ul>

      <p class="pitch">
        I picked up volleyball in June 2024. Within a year I'd made Seaside
        14 Black — the only Seaside team playing Open — and finished 20th at
        Nationals. Next target is an 11'2" approach reach.
      </p>

      <div class="cta-row">
        <a class="btn" href="{{ '/film/' | relative_url }}">Watch Film</a>
        <a class="btn btn-outline" href="{{ '/stats/' | relative_url }}">Full Measurables</a>
        <a class="btn btn-outline" href="{{ '/schedule/' | relative_url }}">Schedule</a>
        <a class="btn btn-outline" href="{{ '/contact/' | relative_url }}">Contact</a>
      </div>
    </div>

    <div class="hero-media">
      {% include video-embed.html %}
    </div>
  </div>
</section>

<section>
  <h2>Explore</h2>
  <ul class="page-list">
    <li><a href="{{ '/stats/' | relative_url }}">Stats / Measurables<span class="desc">Physical and skill numbers, dated.</span></a></li>
    <li><a href="{{ '/film/' | relative_url }}">Film<span class="desc">Highlight reel and full-match links.</span></a></li>
    <li><a href="{{ '/schedule/' | relative_url }}">Schedule<span class="desc">Upcoming tournaments and showcases.</span></a></li>
    <li><a href="{{ '/academics/' | relative_url }}">Academics<span class="desc">GPA, test scores, intended major, NCAA status.</span></a></li>
    <li><a href="{{ '/about/' | relative_url }}">About<span class="desc">How I got here and how I work.</span></a></li>
    <li><a href="{{ '/log/' | relative_url }}">Log<span class="desc">What changed since last season, and when.</span></a></li>
    <li><a href="{{ '/training/' | relative_url }}">Training<span class="desc">The training system behind the numbers.</span></a></li>
  </ul>
</section>
