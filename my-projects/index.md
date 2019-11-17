---
layout: page
title: My Projects
excerpt: "My projects."
search_omit: true
---
{% for post in site.posts  %}
    {% if forloop.first %}
    <h2 id="{{ this_year }}-ref">{{this_year}}</h2>
    <ul>
    {% endif %}

    <li><a href="{{ post.url }}">{{ post.title }}</a></li>

    {% if forloop.last %}
    </ul>
    {% else %}
        {% if this_year != next_year %}
        </ul>
        <h2 id="{{ next_year }}-ref">{{next_year}}</h2>
        <ul>
        {% endif %}
    {% endif %}
{% endfor %}


<ul class="post-list">
{% for post in site.categories.blog %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>
  <!--{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}--></a></article></li>
{% endfor %}
</ul>
