---
layout: default
title: "Film | Victor Deglon"
description: "Highlight reel and full-match film for Victor Deglon, opposite hitter."
permalink: /film/
---

<section>
  <h1>Film</h1>
  <p class="lede">Highlight reel first, full-match film below — for coaches who want the whole game, not just the cut.</p>

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
  <p>
    Full-match film will be listed here by tournament and date as it
    becomes available. If you need game film before then, please
    <a href="{{ '/contact/' | relative_url }}">get in touch</a>.
  </p>
</section>
