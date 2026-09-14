---
layout: default
title: "Film | Victor Deglon"
description: "Highlight reel and full-match film for Victor Deglon, opposite hitter."
permalink: /film/
---

<section>
  <h1>Film</h1>
  <p class="lede">Highlight reel first, full-match links below for coaches who want to see the whole game, not just the highlight package.</p>

  {% include video-embed.html %}

  {% if site.data.profile.video_url != "" %}
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "VideoObject",
    "name": "{{ site.data.profile.name }} — Highlight Reel",
    "description": "Volleyball highlight reel for {{ site.data.profile.name }}, {{ site.data.profile.position }}.",
    "uploadDate": "{{ site.time | date_to_xmlschema }}",
    "embedUrl": {{ site.data.profile.video_url | jsonify }},
    "thumbnailUrl": {{ site.logo | absolute_url | jsonify }}
  }
  </script>
  {% endif %}

  <h2>Full match film</h2>
  <p class="note">
    Hudl coming soon. Once it's up, this section will list full-match
    links by tournament name and date — coaches evaluating seriously
    want game film, not just the highlight cut.
  </p>

  <h2>Timestamped plays</h2>
  <p class="note">
    [Optional but high-value: a short list of timestamps in the reel above
    tied to specific plays — e.g. "0:42 — back-row attack vs. block" —
    so a coach skimming in 15&ndash;30 seconds can jump straight to what
    matters to them.]
  </p>
</section>
