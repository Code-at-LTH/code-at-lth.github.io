---
layout: panel
title: Practice contests
id: practice_contests
---

## Past practice contests

Here you can find a collection of some of the past practice contests we have held, sorted by the algorithm, technique or general theme they focused on.

{% assign sorted_categories = site.data.practice_contests | sort: "category" %}

{% for category in sorted_categories %}

### {{ category.category }}

<ul>
    {% for link in category.links %}
        <li><a href="{{link}}">{{ link }}</a></li>
    {% endfor %}    
</ul>

{% endfor %}
