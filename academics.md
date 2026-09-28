---
layout: default
title: "Academics | Victor Deglon"
description: "GPA, test scores, intended major, and NCAA Eligibility Center status for Victor Deglon."
permalink: /academics/
---

<section>
  <h1>Academics</h1>
  <p class="lede">
    Coaches recruit the whole application, not just the film — academic
    fit and NCAA eligibility status matter as much as measurables at the
    point a program actually offers.
  </p>

  <div class="overflow-table">
  <table class="kv-table">
    <tbody>
      <tr><th scope="row">GPA</th><td>{{ site.data.profile.gpa | default: "TBD" }}</td></tr>
      <tr><th scope="row">Test scores</th><td>{{ site.data.profile.test_scores | default: "TBD" }}</td></tr>
      <tr><th scope="row">Intended major</th><td>{{ site.data.profile.intended_major | default: "TBD" }}</td></tr>
      <tr><th scope="row">High school</th><td>{{ site.data.profile.high_school | default: "TBD" }}</td></tr>
      {% if site.data.profile.coursework != "" %}
      <tr><th scope="row">Coursework</th><td>{{ site.data.profile.coursework }}</td></tr>
      {% endif %}
      {% if site.data.profile.ncaa_id != "" %}
      <tr><th scope="row">NCAA Eligibility Center ID</th><td>{{ site.data.profile.ncaa_id }}</td></tr>
      {% endif %}
      <tr><th scope="row">NCAA status</th><td>{{ site.data.profile.ncaa_status | default: "TBD" }}</td></tr>
    </tbody>
  </table>
  </div>

  <p class="note">
    No AP classes or standardized tests yet, and no NCAA Eligibility Center
    registration — all three come later, which is normal for a class of 2030
    athlete. This page updates as each one happens.
  </p>
</section>
