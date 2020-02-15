---
layout: page
title: About us
permalink: /about/
toggle: on
rank: 3
---

<!--
<div style="margin-bottom: 2em;">
    <img src="{{ 'team/team_paolo.jpg' | prepend: site.images_dir | prepend: site.baseurl }}" />
</div>
-->

Biodatascience101 is a Sino-Danish Center sponsored project dedicated to developing biological data science teaching materials for industry professionals and academics.

Our aim is to provide the teaching environment, networking opportunities and community needed to support current and aspiring data scientists in their biological data-science driven collaborative research projects.

We believe that by focusing on the right fundamental workflows and working closely with real world case data, anyone aspiring to become a data scientist can accomplish their data-driven scientific goals. 

The Biodatascience101 project was started in September 2019, led by Paolo Marcatili, Magnus Haraldson Høie and Andreas Fønns Møller. 

### Our team
<div class="lab-wrapper">
    <ul class="lab-list">
    <!-- Current PIs -->
    {% for member in site.data.team %}
        {% if member.is_current and member.is_pi %}
            {% if member.name and member.bio %}
                {% include member.html %}
            {% endif %}
        {% endif %}
    {% endfor %}
    <!-- Current non-PIs -->
    {% for member in site.data.team %}
        {% if member.is_current and member.is_pi == false %}
            {% if member.name and member.bio %}
                {% include member.html %}
            {% endif %}
        {% endif %}
    {% endfor %}


    </ul>
</div>
