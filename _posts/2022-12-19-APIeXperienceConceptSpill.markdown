---
layout: post
title:  "APIeXprience(AX),Concept Spill: UweFriedrichsen"
date:   2022-12-19 11:28:00 -0400
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
This post caught my attention as I was scrolling through Uwe Friedrichsen's list of blogs. It had API in its subtitle and since we had covered RESTful API's in class I though this would be a great opportunity to see his approach to API design. After scanning through the blog I saw the term concept spill which I had not heard before and I thought it would be interesting to learn something new about API through the lens of an experienced IT specialist.

## Summary of the post
The author begins by talking about how by taking technologies and fitting them into the entire system might work easily but we end up missing the important aspect of fully fullfilling the users needs. He introduces a concept AX which reffers to APIeXperience as to how the programmer will be able to work with an API design to fulfill the requirements of his users. Similar to UX in application design, a good AX might breed good results on the operational and functional side of a system or system software. He then introduces concept spill which is one of the factors that might reduce the AX of a programmer.

He defines concept spill as a situation where, "in order to use another service to solve your acutal problem, you first need to understand its internal concepts." He gives a good example of how you would have to understand a city's transport systems, such as zones, bus and train stops etc., when you want to move from one point to another in a new city. You are force to understand the city's layout before you solve your initial problem of going to a particular place within the city, concept spill.

Concept spill pours over into the IT world in API design where a programmer is forced to learn how the creators of the API came up with the API's stucture and inner workings on top of the issue that he is trying to solve. How do we solve the problem of concept spill? At the root of avoiding concept spill is to understand the user's needs and design your API to cater for the user's needs. An API designed without the user's context/story in mind will lead to poor operations of the API thus futher complications. Understand common uses of the API and base your design on these uses. 

## Reflection and Application
The blog post offered good advice on how to make API more user based which makes good design and acceptance by developers. Even as I look forward to working on my software capstone next semester, I think this will be great to put in mind as we work on improving Thea's Pantry.
