---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

<h2>Pages</h2>
<ul>
  <li><a href="{{ base_path }}/">Home</a></li>
  <li><a href="{{ base_path }}/publications/">Publications</a></li>
  <li><a href="{{ base_path }}/teaching-talks-press/">Teaching, Talks, &amp; Press</a></li>
  <li><a href="{{ base_path }}/cv/">CV</a></li>
</ul>

<h2>Publications</h2>
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<h2>Talks</h2>
{% assign sorted_talks = site.talks | sort: "date" | reverse %}
{% for post in sorted_talks %}
  {% include archive-single.html %}
{% endfor %}

<h2>Teaching</h2>
{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}
