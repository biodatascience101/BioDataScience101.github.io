---
layout: page
title: Events
permalink: /events/
toggle: on
rank: 4
---

For more information about the below events, please click the links below or contact **admin@example.com**.


### Current event calendar:
- DTU Pilot event, Copenhagen 2020 - February 2020
- SDC Pilot event, Copenhagen 2020 - April 2020
- 1st BioDataScience101 Workshop, Copenhagen - June 2020
- 2nd BioDataScience101 Workshop, Beijing - September 2020
- 3rd BioDataScience101 Workshop, Bangalore - November 2020


<ul class="post-list">
    {% for post in site.posts reversed %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>


