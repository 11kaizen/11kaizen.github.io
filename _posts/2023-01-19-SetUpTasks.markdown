---
layout: post
title:  "Libre Food Pantry and Thea's Pantry"
date:   2023-01-19 16:48:00 -0400
categories: [CS@Worcester, CS-448, Set-upTask3]
---
<div class="post-categories">
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.baseurl}}/categories/#{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>


I chose to write about licensing because it is a topic that is least explored by most students. Since Libre Food Pantry is an open source software its licensing is pretty much similar to Linux's licenses. Libre Food Pantry is formed on the foundations of General Public License, that are reffered to as the four freedoms. The software remains free to all no matter the modifications or changes in ownership that are made to it. GPLv3 is an improved version of the original GPL to keep ip upto date with newer policies such as the Digital Millenium Copyright Act.

First of all I am impressed by how well documented the software is, the explanations within the readme are concise. After exploring the architecture of Thea's Food Pantry, I am curious to see how we will be able to intergrate our work together considering that we are three different groups working on standalone components of the software. The workflow section was also fun to read about. The sequence of events were the actual ones that we took as we did the first activity in class. I think that overall it will be a great experience working on Thea's Pantry as it will prepare us for real world application I look forward to a productive semester!
