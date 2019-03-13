---
layout: panel-with-sidebar
title: Home
---

## Welcome

Welcome to the homepage of Code@LTH!

## About
{% include about.html %}

You can read more about Code@LTH on our [About page](/about).


## Events

You can find all our events on [Facebook](https://www.facebook.com/CodeAtLTH/events).


## Blog Posts
<ul class="posts">
    {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
