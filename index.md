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

      <ul class="facts">
        <li><strong>Position:</strong> {{ site.data.profile.position }}</li>
        <li><strong>Class:</strong> {{ site.data.profile.class_year | default: "TBD" }}</li>
        <li><strong>Height:</strong> {{ site.data.profile.height | default: "TBD" }}</li>
        <li><strong>Approach Reach:</strong> {{ site.data.stats[2].current }}</li>
      </ul>

      <p class="note">
        <strong>One-line pitch:</strong> [Add a single sentence here — the
        specific thing a coach should remember: e.g. "Opposite with a 10'5"
        touch reach and a serve that's forcing errors at the open club level."
        Numbers, not adjectives — see the pushback on superlatives in the
        <a href="{{ '/about/' | relative_url }}">About</a> page.]
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
    <li><a href="{{ '/about/' | relative_url }}">About<span class="desc">Bio, work ethic, leadership.</span></a></li>
    <li><a href="{{ '/log/' | relative_url }}">Log<span class="desc">Dated updates after every tournament and PR.</span></a></li>
    <li><a href="{{ '/training/' | relative_url }}">Training<span class="desc">The training system behind the numbers.</span></a></li>
  </ul>
</section>
