---
layout: default
title: "Stats / Measurables | Victor Deglon"
description: "Dated physical and skill measurables for Victor Deglon, opposite hitter: vertical jump, reach, serve speed."
permalink: /stats/
---

<section>
  <h1>Stats / Measurables</h1>
  <p class="lede">
    Current numbers, goals, and the date each was last verified. Updated
    after every testing session — see the <a href="{{ '/log/' | relative_url }}">Log</a>
    for the training context behind each change.
  </p>

  <div class="responsive-table">
  <table>
    <caption>Physical measurables</caption>
    <thead>
      <tr><th>Metric</th><th>Current</th><th>Goal</th><th>Last updated</th><th>Context</th></tr>
    </thead>
    <tbody>
      {% for row in site.data.stats %}
      <tr>
        <td data-label="Metric">{{ row.metric }}</td>
        <td data-label="Current">{{ row.current }}</td>
        <td data-label="Goal">{{ row.goal | default: "—" }}</td>
        <td data-label="Last updated">
          {% if row.last_updated contains "-" and row.last_updated.size == 10 %}
          <time datetime="{{ row.last_updated }}">{{ row.last_updated }}</time>
          {% else %}
          {{ row.last_updated }}
          {% endif %}
        </td>
        <td data-label="Context">{{ row.context | default: "—" }}</td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
  </div>

  <h2>For reference</h2>
  <p>
    Published D1 benchmark data: D1 outside hitters average roughly a
    118-inch approach jump. Opposite-specific public benchmarks are thin,
    so this is the closest comparable — worth knowing where an
    11'2"&ndash;11'6" approach/touch reach range lands relative to it as
    that number climbs.
  </p>

  <h2>Skill numbers</h2>
  <p class="note">
    [Add hitting percentage, kill efficiency, serve-receive rating, or
    other stat-line numbers here once available from match/tournament
    data — with the same dated format as the table above.]
  </p>
</section>
