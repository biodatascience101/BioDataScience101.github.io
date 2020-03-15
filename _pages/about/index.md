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
<p style="text-align:justify">
-->
<p style="text-align:justify">
BioDataScience101 is an educational project dedicated to enabling practical use of fundamental biological data science analyses for industry professionals, students and academics.
<br>
Our aim is to provide an inspired teaching environment taught by academic and industry experts, the toolbox for fundamental workflows and the community needed to train new as well as current biological data scientists in their data-science driven collaborative research projects. 
<br>
We believe that by focusing on fundamental workflows, working hands-on with scientific case data and closely with academic and industry experts, anyone aspiring to become a biological data scientist can accomplish their data-driven scientific goals. 
<br>
The BioDataScience101 project was started in September 2019, led by Paolo Marcatili, Magnus Haraldson Høie and Andreas Fønss Møller. </p>

<br />
# Teaching committee:
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
  <hr>
  

 <br>
 <h3 class="center">This work is made possible through generous support from: </h3>
   <br>
    <div class="row"> 
      <div class="column_left">
          <a href="https://www.dtu.dk">
        <img src="{{ 'DTU.png' | prepend: site.images_dir | prepend: site.baseurl }}">
          </a>
       </div>
       <div class="column_right">
         <a href="https://danishhealthtech.dk">
         <img src="{{ 'Logo_Danish_helthtech.png' | prepend: site.images_dir | prepend: site.baseurl }}"  width="200%">
         </a>
         <a href="https://www.welfaretech.dk">
         <img src="{{ 'Logo_welfare_tech.png' | prepend: site.images_dir | prepend: site.baseurl }}"  width="200%">
         </a>
         <a href="https://ec.europa.eu/regional_policy/da/funding/erdf/">
         <img src="{{ 'Logo_EU.png' | prepend: site.images_dir | prepend: site.baseurl }}"  width="200%">
         </a>
        </div> 
    </div>
   </div>
