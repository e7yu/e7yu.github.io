---
layout: page
permalink: /publications/
title: Publications
description: 
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

Detailed publication information is also availiable at my <a href="https://scholar.google.com/citations?user=vNMZtRMAAAAJ" target="_blank" rel="noopener noreferrer">Google Scholar</a> page.

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications" style="max-width: 900px; margin: 0 auto;">

<!-- JOURNAL HEADER -->
<h2 style="text-align: center; font-size: 1.6rem; margin-top: 3rem; margin-bottom: 1rem;">
Journal Articles
</h2>

<div class="pub-section" style="margin-bottom: 3.5rem;">
  {% bibliography --query @*[keywords=J] %}
</div>

<!-- spacing between sections is handled here -->
<div style="height: 1.5rem;"></div>

<!-- CONFERENCE HEADER -->
<h2 style="text-align: center; font-size: 1.6rem; margin-bottom: 1rem;">
Peer-reviewed Conference Proceedings & Published Abstracts
</h2>


  {% bibliography --query @*[keywords=C] %}


</div>
