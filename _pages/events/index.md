---
layout: page
title: Events
permalink: /events/
toggle: on
rank: 4
---

For more information about the below events, please click the links below or contact <admin>.

### BioDataScience101 DTU pilot event: Copenhagen, Denmark February 2020

### BioDataScience101 SDC pilot event: Copenhagen, Denmark April 2020

### 1st BioDataScience101 Workshop: Copenhagen, Denmark June 2020

### 2nd BioDataScience101 Workshop: Beijing, China September 2020

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


