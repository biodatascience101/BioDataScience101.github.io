---
layout: page
title: AboutUs
permalink: /about/
toggle: on
rank: 4
---

<!--
<div style="margin-bottom: 2em;">
    <img src="{{ 'team/team_paolo.jpg' | prepend: site.images_dir | prepend: site.baseurl }}" />
</div>
-->

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
