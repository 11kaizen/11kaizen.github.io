---
layout: post
title:  "The Non-Existence of ACID consistency: UweFriedrichsen"
date:   2022-12-4 21:00:00 -0400
categories: [CS@Worcester, CS-343, Week-12]
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
I selected the blog as the author who has years of experience again highlight a key barrier that exists within distributed systems which can mirror microservices architecture. The two have to independent but interdependent qualities and a change to one part of the system will likely affect the entire system. The blog also addresses architecture of systems which is key in considering the design and the policies that are to be implemented across a number of systems.The author also has a good scientific approaches as to how to determine the success rate of an update upon a number of systems as well the breakdown as to how he arrived at such conclusions.

## Summary of the post
The author introduces the concept of ACID consistency in business where a change in one part of a system should reflect across all other parts of the business. ACID is defined as the atomicity, consistency, isolation and durability and it is mostly implemented in database transactions to ensure data validity despite errors, power failures and other mishaps. Atomicity guarantees that each transaction is treated as a single unit that succeeds completly or fails completely. Consistency ensures that a transaction can only bring the database from one consistency state to another. Isolation ensures that concurrent execution of transactions leaves the database in the same state that would have been obtained if the transactions were executed sequentially. Finally, durability gurantees that once a transaction has been committed, it will remain committed even in the case of a system failure. The author focuses on why it is important that consistency is established across multiple systems. Considering the number of applications that companies use in the world today, along with the number of paths of communication in these organizations, establishing consistency is an uphill task. "The more systems involved the higher the chance of a failure." In comparison with older systems when may of the connections were batch-type, the systems today which have online communicaition paths are more prone to errors. Batch-type systems were considered to be more more tolerant. 


## Reflections and application 
Again Friedrichsen offers good insight as to how hard it is to establish consistency across multiple distributed systems. Considering factors such as down time and the success rate when carrying out updates, establising consistency becomes a challenging task, I look forward to seeing some of the solutions or ways of ensuring consistency that he offers in the following blog as I believe that this is a huge challenge that most businesses face today. I have learnt that establishing consistency within systems is vital but it prooves challenging as the number of systems and communication paths between them grow.
