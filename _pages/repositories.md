---
layout: page
permalink: /repositories/
title: repositories
description: Some of my most recent projects with code and derivations.
nav: true
nav_order: 3
---

{% if site.data.repositories.github_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
