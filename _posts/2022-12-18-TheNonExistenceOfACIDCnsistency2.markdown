---
layout: post
title:  "The Non-Existence of ACID consistency 2: UweFriedrichsen"
date:   2022-12-17 12:00:00 -0400
categories: [CS@Worcester, CS-343, Week-14]
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
I chose this post because I find that Uwe Friedrichsen's insights are usually revealing and an accurate description of what I am to encounter in my work life. This topic, surrounding ACID consistency, is also closely related with software architecture as most systems work in unison nowadays due to the structure of microservices in most systems. Above all he gives real life examples that support his claims in a logical and meaningful manner. His structure of developing arguments with more than one blog post is also great as it slowly build up claims with good evidences and examples.

## Summary of post
Friedrichsen begins by introducing the concept of eventual consistency and compares it to strong consistency. He talks about an example of money transfer between two people and how it takes time for the money to reflect on the recipients account. Strong consistency would mean that immediately the money is transferred there would be a reception on the recipients end, however, eventual consistency is what we have where after a while where the money eventually reflects after a period time.

The author again gives another example of how strong consistency is non-existent. In this example a clerk gets called by a customer who needs some infomation, the clerk retrieves data need to answer the question and gets it displated on the screen. As he goes through the information before he answers the customer the data changes and the author poses a question,"Will the answer of the clerk be based on the current data? Or will the answer be based on the old data that was valid until some seconds ago but is invalid now?" This again show the incosistent nature of data and therefore the non-existence of a strongly consistent system. 

## Reflections and application
The author makes a valid argument on the non-existence of strong consistency. I understood the difference between strong and eventual consistency. I also realized that all systems today run on eventual consistency. We do not have a guarantee of the outcome but it is after time that we eventually get consistency. 

This concept reminds me that we can never achieve perfection and reminds me that progress matters more than perfection not only in our careers but in our daily lives as well. So as I work on projects invlolving systems I would focus more on having the individual parts communicate and then gradually improve their performance as time progresses.
