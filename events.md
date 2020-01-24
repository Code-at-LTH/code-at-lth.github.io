---
layout: base
id: events
title: Events
---

# Events

We plan to host all events here. However currently a lot of old events only exists on Facebook.

{% assign events = site.events | sort: "date" | reverse  %}
{% for e in events  %}
## [{{e.title}}]({{e.redirect | default: e.url}}) 
##### {{e.date | date_to_string}}
{% endfor %}
