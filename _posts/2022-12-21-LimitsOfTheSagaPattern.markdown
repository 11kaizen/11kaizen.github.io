---
layout: post
title:  "LimitsOfTheSagaPattern: UweFriedrichsen"
date:   2022-12-21 20:48:00 -0400
categories: [CS@Worcester, CS-343, Week-15]
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
This post intrigued me as it talked about microservices and since we had worked with the microservices that are makeup Thea's Pantry it was a great opportunity to learn something new concerning microservices. Saga pattern was also a new concept that I had not heard or implemented before. Considering earlier posts that I had done with Friedrichsen I was sure that he would give good and relevant examples to understand the topic. 

## Summary of the post
Friedrichsen begins by introducing the concept, saga pattern. He describes it as, "if you have a transaction that spans multiple services and thier database, do not use distributed transaction. User the Saga pattern instead: Call the affected services in a row - tupically by using events for activity propagation." 

The author then goes to explain how the saga pattern might lead to limitation within a microservices systems due to technical errors. Despite the ability of the saga pattern to cover roll backs, Freidrichsen talks about how if a roll back fails it might lead to larger errors which cannot be solved. The main technique used to handle technical errors is to have a copy of the changes that were to be applied, go back to the last checkpoint by loading the last snapshot and then retrying application of the changes while avoiding the potential error that initially led to the technical error.

Saga's pattern strength is in recovering from business error rather than technical errors. Friedrichsen states that recovering from technical error invovles a two layer approach where there is a lower layer which is hidden from the upper business layer. Also Friedrichsen cautions that if the saga pattern is used too often there might be an existing design smell within the system.

## Reflection and Applicaition
As I have learnt about how important it is to consider the limitations and the advantages of using certain design patterns. In this case the strength of the saga pattern was in handling business errors but its downside was in handing technical errors. Also frequent application of a certain design might be a sign of an underlying problems which might require diagnosis. I also learnt of how the business and the technical layer can interact and work together and how to hide the functionality of the technical layer from the business layer.

I would apply the concepts that I have learnt from this post as I design systems which involve microservices. I will be careful to examine the pros and cons that different technologies might have before implementing them and relying on them to carry out roles within the entire system.
