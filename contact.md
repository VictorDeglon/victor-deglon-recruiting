---
layout: default
title: "Contact | Victor Deglon"
description: "Recruiting contact for Victor Deglon, opposite hitter."
permalink: /contact/
---

<section>
  <h1>Contact</h1>
  <p class="lede">
    For recruiting inquiries, please reach out using the contact below.
  </p>

  <div class="overflow-table">
  <table class="kv-table">
    <tbody>
      <tr><th scope="row">Recruiting email</th><td><a href="mailto:{{ site.data.profile.recruiting_email }}">{{ site.data.profile.recruiting_email }}</a></td></tr>
      {% if site.data.profile.recruiting_phone != "" %}
      <tr><th scope="row">Phone</th><td>{{ site.data.profile.recruiting_phone }}</td></tr>
      {% endif %}
      <tr><th scope="row">Club team</th><td>{{ site.data.profile.club_team | default: "TBD" }}</td></tr>
      {% if site.data.profile.maxpreps_url != "" %}
      <tr><th scope="row">MaxPreps</th><td><a href="{{ site.data.profile.maxpreps_url }}">{{ site.data.profile.maxpreps_url }}</a></td></tr>
      {% endif %}
    </tbody>
  </table>
  </div>

  <p class="note">
    A phone number isn't listed yet — add one in
    <code>_data/profile.yml</code> when you're ready, ideally a
    parent's or coach's number rather than a personal cell.
  </p>
</section>
