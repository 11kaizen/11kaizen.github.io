---
layout: post
title:  "The 100% Availablity Trap: UweFriedrichsen"
date:   2022-10-30 21:00:00 -0400
categories: [CS@Worcester, CS-343, Week-7]
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

## Why I chose this post 
As we have progressed with the course material we have seen the advantages that microsystems have over monolithic structured systems. These advantages have shown to overcome most of the limitations that monolithic structures exhibited. However, microsystems or distributed softwares have some short comings of their own. In this blog the author focuses on some of the errors that may arise within a distributed software.This would shed some light on some of the cons of microsystems.

## Summary of the post
The author begins by speaking about the 100% availablity trap which most developers fall into. This trap is where developers, " assume that all remote peers, icluding infrastructure tools like databases, message brokers and alike , are available 100% of the time, i.e., that they are never down." The author breaks down why a distributed system cannot be available for 100% of the time. A system is not available if it does not respond, responds slower that specified or provides a wrong response. The author then mentions the "nines" which looks at what a 90% and above availability looks like for a distributed system. To get to these levels of availability there is a lot of consideration that goes into play, from patch and maintenance days to managing test and runtime which will drastically increase to achieve this level of availablity. Not forgetting the costs and efforts.

The author then alludes to the fact that with increasing number of nodes there is an expected decrease in the availability of the system as well. Also another factor to cosnsider is the network that facilitates communication between the nodes. The network must be in perfect condition to ensure perfect availability which is very hard to actualize.

Finally the author ends with this statement. "The question is not, if failures will hit you in a distributed system landscape.The only question left is, when and how bad they will hit you."

## Reflections and application 
Despite the countless number of advantages that a distributed system has, I have realized that they cannot achieve perfection. "Every dog has its own fleas." The author has clearly shown me how this is true. The final remark that he has also brings in a perspective of always being ready to experience an issue. These concepts that I have learnt I'm sure will prove valuable and important in my career life and even as I work on projects that involve microservices.
