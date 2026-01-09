---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all pages and content on this site. For robots, an [XML version]({{ base_path }}/sitemap.xml) is available.

## Main Pages

- [Home]({{ base_path }}/) - About me and research overview
- [About]({{ base_path }}/about/) - Detailed background and experience
- [Publications]({{ base_path }}/publications/) - Academic publications
- [Research]({{ base_path }}/research/) - Research projects and interests
- [Projects]({{ base_path }}/projects/) - Software and engineering projects
- [Blog]({{ base_path }}/blog/) - Blog posts and articles
- [CV]({{ base_path }}/files/shreeram_gs%20Resume.pdf) - Curriculum Vitae

## Browse By

- [Categories]({{ base_path }}/categories/) - Posts organized by category
- [Tags]({{ base_path }}/tags/) - Posts organized by tag

## Publications

{% for post in site.publications %}
- [{{ post.title | strip_html }}]({{ base_path }}{{ post.url }})
{% endfor %}

## Research

{% for post in site.research %}
- [{{ post.title | strip_html }}]({{ base_path }}{{ post.url }})
{% endfor %}

## Projects

{% for post in site.project %}
- [{{ post.title | strip_html }}]({{ base_path }}{{ post.url }})
{% endfor %}

## Blog Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ base_path }}{{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
