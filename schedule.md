---
layout: default
title: "Schedule | Victor Deglon"
description: "Upcoming tournaments and showcases for Victor Deglon, opposite hitter."
permalink: /schedule/
---

<section>
  <h1>Schedule</h1>
  <p class="lede">
    Club tournaments are where coaches do most in-person evaluation — this
    page is kept current for that reason. Edit
    <code>_data/schedule.yml</code> to add or remove events.
  </p>

  {% if site.data.schedule.size > 0 %}
  <div class="overflow-table">
  <table>
    <thead>
      <tr><th>Event</th><th>Date</th><th>Location</th><th>Club / Division</th></tr>
    </thead>
    <tbody>
      {% for e in site.data.schedule %}
      <tr>
        <td>{% if e.url != "" %}<a href="{{ e.url }}">{{ e.event }}</a>{% else %}{{ e.event }}{% endif %}</td>
        <td>
          <time datetime="{{ e.date }}">{{ e.date | date: "%b %-d, %Y" }}</time>
          {% if e.end_date %}&ndash; <time datetime="{{ e.end_date }}">{{ e.end_date | date: "%b %-d, %Y" }}</time>{% endif %}
        </td>
        <td>{{ e.location }}</td>
        <td>{{ e.club_team }}{% if e.division != "" %} &middot; {{ e.division }}{% endif %}</td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
  </div>
  {% else %}
  <p class="note">
    No events posted yet. Add entries to <code>_data/schedule.yml</code> —
    event name, date, location, club team, and division.
  </p>
  {% endif %}
</section>
