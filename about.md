---
layout: panel-with-sidebar
title: About
id: about
---

# About

{% include about.html %}

We are always looking for people who are interested in participating and improving our organisation.
If you have ideas about more cool things to organize with us, or you just want to hang out, feel free to
contact us by sending one of us an email (or message us on facebook). That way we can invite you to our weekly meetings, that usually are at lunchtime on Tuesdays.


If you are interested more in detail about how our organisation works, have a look at our documents in our [meta repository](https://github.com/Code-at-LTH/meta).
There you can find our [by-law](https://en.wikipedia.org/wiki/By-law), operational plan, etc. 

## Board members 2020
<div class="row">
    {% for member in site.data.members %} {% if member.current == true %}

    <div class="col-xs-6 col-sm-4 col-md-4 col-lg-3">
        <div class="thumbnail">
            {% if member.img %}
            <img class="contact-image" src="{{ member.img }}" alt="{{ member.name }}">
            {% endif %}
            <div class="caption">
                <h4>{{ member.name }}</h4>
                <p> {{ member.role }}</p>
                {% if member.github %}
                <p> <a href="https://github.com/{{ member.github }}" target="_blank"> @{{ member.github }} </a> </p>
                {% endif %}
                <h2> 
                {% if member.mail %}
                <a href="mailto:{{ member.mail }}"><i class="fa fa-envelope-square"></i></a> 
                {% endif %}
                {% if member.github %}
                <a href="https://github.com/{{ member.github }}" target="_blank"><i class="fa fa-github-square"></i></a>
                {% endif %}
                {% if member.website %}
                <a href="https://{{ member.website }}" target="_blank"><i class="fa fa-home"></i></a>
                {% endif %}
                </h2> 
            </div>
        </div>
    </div>
    {% assign mod4 = forloop.index | modulo:4 %}
    {% assign mod3 = forloop.index | modulo:3 %}
    {% assign mod2 = forloop.index | modulo:2 %}
    {% if mod2 == 0 %}
    <div class="clearfix visible-xs-block"></div>
    {% endif %}
    {% if mod3 == 0 %}
    <div class="clearfix visible-sm-block"></div>
    <div class="clearfix visible-md-block"></div>
    {% endif %}
    {% if mod4 == 0 %}
    <div class="clearfix visible-lg-block"></div>
    {% endif %}

    {% endif %}{% endfor %}
</div>

## Previous Board members
<div class="row">
    {% assign index = 1 %}
    {% for member in site.data.members %} {% if member.current != true %}
    <div class="col-xs-6 col-sm-4 col-md-4 col-lg-3">
        <div class="thumbnail">
            <div class="caption">
                <h4>{{ member.name }}</h4>
                <p> {{ member.role }}</p>
                <p> <a href="https://github.com/{{ member.github }}" target="_blank"> @{{ member.github }} </a> </p>
            </div>
        </div>
    </div>
    {% assign mod4 = index | modulo:4 %}
    {% assign mod3 = index | modulo:3 %}
    {% assign mod2 = index | modulo:2 %}
    {% if mod2 == 0 %}
    <div class="clearfix visible-xs-block"></div>
    {% endif %}
    {% if mod3 == 0 %}
    <div class="clearfix visible-sm-block"></div>
    <div class="clearfix visible-md-block"></div>
    {% endif %}
    {% if mod4 == 0 %}
    <div class="clearfix visible-lg-block"></div>
    {% endif %}
    {% assign index = index | plus:1 %}
    {% endif %}{% endfor %}
</div>
