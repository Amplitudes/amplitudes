---
permalink: /theses/
layout: splash
title: "Amplitudes Related Ph.D Theses"
modified: 2019-06-18
header:
  overlay_color: "#5e616c"
  overlay_image: sixPtRelations.jpg
  overlay_filter: .4
  caption: ""
author_profile: false
---

## Amplitudes Related PhD Links

This originally started as a repository for SAGEX theses -- but other amplitudes related PhD folk are welcome to link to their dissertations.

{% capture site_categories %}{% for tag in site.categories %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
<!-- site_categories: {{ site_categories }} -->
{% assign tag_words = "theses,null" | split:',' %}
{% assign firstWord=tag_words[0] %}
{% assign secondWord=tag_words[-1] %}
<!-- first: {{ firstWord }} -->
<!-- second: {{ secondWord }} -->
<!-- tag_words: {{ tag_words }} -->

<div id="categories">

  {% for item in (0..site.categories.size) limit:2 %}{% unless forloop.last %}
    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}
  <ul class="posts">
    {% for post in site.categories[this_word] %}{% if post.title != null %}
    <li itemscope><span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time></span> &raquo; <a href="{{ post.url }}">{{ post.excerpt }}: {{ post.title }}</a></li>
    {% endif %}{% endfor %}
  </ul>
  {% endunless %}{% endfor %}
</div>
