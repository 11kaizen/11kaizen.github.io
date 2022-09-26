---
layout: post
title:  "Resilience: UweFriedrichsen"
date:   2022-09-25 21:00:00 -0400
categories: [CS@Worcester, CS-343, Week-2]
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
Considering the experience of the author, Uwe Friedrichsen, who is a CTO at codecentric along with years of experience. I was intrigued why he would write a blog series on the topic of resilience in software design. I figured that this would be a key concept in designing software and therefore I decided to read the blog. As I read through the blog the author mentioned concepts that we would be covering in class such as API and other new concepts such as service meshes which motivated me to read more. 
## Summary of the post
The author begins by defining what resilience is. He defines it as keeping correct operation in the face of unexpected events or at least recovering from them in a timely manner, while offering a gracefully degraded service in the interim. He then goes into a quick run through of how the matter of resilience was left to the operations teams in the past.

Developers would develop software with an apporach that it was running a single process on a single machine that will never fail. Nowadays, container schedulers are making sure a specified number of replicas are active, service meshes offering timeout and monitoring automatic retries along with API gateways taking care of rate limiting and failover showing that the concept is still prevalent.

Friedrichsen then shows how distributed systems came to change the whole mentality of "running a single process on a single machine that will never fail". He explains this With an example of how batch processes took the place of data typists and eventually became overtaken due to the internet and remote procedure calls (RPC). He goes on futher to show that the increase of the number of devices in the Iot has led to an increased number of peers on the systems leading to further implementation of distributed systems. He concludes by speaking about how softwares are running 24/7 which puts more need on the dependance of distributed systems.


## Reflections and application 
Being the first part of the blog series, the author introduces the importance of distributed systems and shows its growth through history well. I personally learnt how important distributed systems are in running most of the softwares that we run today, conisering that fridges can now be part of the internet. As we begin the process of learning how to design software I will keep this principle in the back of my mind that resilience is important in software construction.


