---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
excerpt: "Education, experience, publications, and teaching in one place."
redirect_from:
  - /resume
---

{% include base_path %}

<section class="cv-section">
  <h2 class="archive__section-title">Education</h2>
  <div class="cv-entry">
    <h3>M.S. in Applied Statistics</h3>
    <p>University of Science and Technology of China, 2024</p>
  </div>
  <div class="cv-entry">
    <h3>B.S. in Mathematics and Applied Mathematics</h3>
    <p>University of Science and Technology of China, 2021</p>
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Work Experience</h2>
  <div class="cv-entry">
    <h3>Teaching Assistant</h3>
    <p>Probability and Mathematical Statistics · 2022.09-2023.02</p>
    <ul class="cv-list">
      <li>Duties included homework correcting and exercise lectures.</li>
      <li>Instructor: Professor Zhishui Hu.</li>
    </ul>
  </div>
  <div class="cv-entry">
    <h3>Internship</h3>
    <p>Supply Chain Y, JD.com · 2022.11-2023.03</p>
    <ul class="cv-list">
      <li>Duties included supply chain causal analysis.</li>
    </ul>
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Publications</h2>
  <div class="cv-collection">
    {% for post in site.publications reversed %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Teaching</h2>
  <div class="cv-collection">
    {% for post in site.teaching reversed %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </div>
</section>
