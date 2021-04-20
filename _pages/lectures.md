---
permalink: /lectures/
layout: splash
title: "Lectures"
modified: 2019-06-18
header:
  overlay_color: "#5e616c"
  overlay_image: sixPtRelations.jpg
  overlay_filter: .4
  caption: ""
author_profile: false
---

## Passports to the future...

{% capture site_categories %}{% for tag in site.categories %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
<!-- site_categories: {{ site_categories }} -->
{% assign tag_words = "lectures,null" | split:',' %}
{% assign firstWord=tag_words[0] %}
{% assign secondWord=tag_words[-1] %}
<!-- first: {{ firstWord }} -->
<!-- second: {{ secondWord }} -->
<!-- tag_words: {{ tag_words }} -->

<div id="categories">

  {% for item in (0..site.categories.size) limit:2 %}{% unless forloop.last %}
    {% capture this_word %}{{ tag_words[item] | strip_newlines }}{% endcapture %}
  <h2 id="{{ this_word | cgi_escape }}">{{ this_word }}</h2>
  <ul class="posts">
    {% for post in site.categories[this_word] %}{% if post.title != null %}
    <li itemscope><span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time></span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}{% endfor %}
  </ul>
  {% endunless %}{% endfor %}
</div>
