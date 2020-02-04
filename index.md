---
layout: panel-with-sidebar
title: Home
---

## Welcome

Welcome to the homepage of Code@LTH!

## About
{% include about.html %}

You can read more about Code@LTH on our [About page](/about).


## [Events](/events)


{% assign events = site.events | sort: "date" | reverse | slice: 0, 3  %}
{% for e in events  %}
### [{{e.title}}]({{e.redirect | default: e.url}}) 
##### {{e.date | date_to_string}}
{% endfor %}

[All events](/events)


## Blog Posts
<ul class="posts">
    {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
