---
layout: base
id: events
title: Events
---

# Events

We plan to host all events here. However currently a lot exists on only Facebook.

{% assign events = site.events | sort: "date" | reverse  %}
{% for e in events  %}
## [{{e.title}}]({{e.url}}) 
##### {{e.date | date_to_string}}
{% endfor %}
