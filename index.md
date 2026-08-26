---
layout: default
title: Monthly Tech & AI News
---

# Monthly Tech & AI News

Welcome to Common Devops AI's monthly news archive. We track the latest developments in AI models, tech industry trends, and emerging technologies.

## Latest Articles

{% assign posts = site.pages | where_exp: "p", "p.name contains '.md' and p.name != 'index.md'" | sort: "name" | reverse %}

<ul>
{% for post in posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title | default: post.name | remove: '.md' | replace: '-', ' ' | capitalize }}</a>
  </li>
{% endfor %}
</ul>

## About

This site is maintained by [Common Devops AI](https://github.com/comdevopsai). Content is generated and curated with the help of Hermes Agent.

---

*Automatically updated via GitHub Actions*
