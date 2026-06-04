---
layout: page
permalink: /connect/
title: Connect
description: 
nav: false
---

<p style="text-align: center;">Reach me by email or through one of the following platforms!
</p>

<div class="connect-page">
  <div class="connect-grid">
    {% for social in site.data.socials %}
      {% case social[0] %}

        {% when "email" %}
          <a class="connect-card"
             href="mailto:{{ social[1] | encode_email }}">
            <i class="fas fa-envelope" style="color:var(--global-theme-color)"></i>
            <span>Email</span>
          </a>

        {% when "linkedin_username" %}
          <a class="connect-card"
             href="https://www.linkedin.com/in/{{ social[1] }}"
             target="_blank"
             rel="noopener noreferrer">
            <i class="fab fa-linkedin" style="color:#0a66c2"></i>
            <span>LinkedIn</span>
          </a>

        {% when "github_username" %}
          <a class="connect-card"
             href="https://github.com/{{ social[1] }}"
             target="_blank"
             rel="noopener noreferrer">
            <i class="fab fa-github" style="color:var(--global-text-color)"></i>
            <span>GitHub</span>
          </a>

        {% when "scholar_userid" %}
          <a class="connect-card"
             href="https://scholar.google.com/citations?user={{ social[1] }}"
             target="_blank"
             rel="noopener noreferrer">
            <i class="ai ai-google-scholar" style="color:#4285f4"></i>
            <span>Google Scholar</span>
          </a>

        {% when "orcid_id" %}
          <a class="connect-card"
             href="https://orcid.org/{{ social[1] }}"
             target="_blank"
             rel="noopener noreferrer">
            <i class="ai ai-orcid" style="color:#a6ce39"></i>
            <span>ORCID</span>
          </a>

      {% endcase %}
    {% endfor %}
  </div>
</div>