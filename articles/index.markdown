---
layout: page
title: Articles
menuitem: yes
---

List of articles grouped by category.

{% for node in site.pages %}
  {% if node.title != nil %}
<li><a href="{{node.url}}">{{node.title}}</a>({{node.category | join: ' '}})</li>
  {% endif %}
{% endfor %}

<!-- {% for category in site.categories %} -->
<!--   <li><a name="{{ category | first }}">{{ category | first }}</a> -->
<!--     <ul> -->
<!--     {% for posts in category %} -->
<!--       {% for post in posts %} -->
<!--         {% if post.title != nil %} -->
<!--         <li><a href="{{ post.url }}">{{ post.title}}</a></li> -->
<!--         {% endif %} -->
<!--       {% endfor %} -->
<!--     {% endfor %} -->
<!--     </ul> -->
<!--   </li> -->
<!-- {% endfor %} -->
