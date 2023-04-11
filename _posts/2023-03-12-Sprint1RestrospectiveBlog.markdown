---
layout: post
title:  "Retrospective Blog: Sprint - 1"
date:   2023-03-19 20:30:00 -0400
categories: [CS@Worcester, CS-448, Sprint-1]
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

At the end of the first sprint our team has become more united and have continually learnt how to work together. Some of the activity that I did on my gitlab include, merging and approving request as in the [link](https://gitlab.com/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/reportingbackend/-/merge_requests/3), [link2](https://gitlab.com/dashboard/merge_requests?scope=all&state=all&assignee_username=11kaizen) this allowed the changes made to the branches of the reporting backend to be consolidataed and put into the main branch. I also used gitlab in picking up issues and checking the status of [other issues that were begin worked on](https://gitlab.com/groups/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/-/boards)

I was really impressed of the way we communicated with each other throughout the sprint. Despite this being the first time that we worked together, for most us. We were able to have healthy communication. This helped us overcome challenges that had faced most us during the sprint. Utilizing platfroms such as discord and personal chats also allowed us to know when one of the members would not be able to make it for the class session. We also relied heavily on each other when we encountered any road blocks as we worked on the issues assigned to us. In an example, the pipeline which had a number of us stuck required almost all of us to jump on that one issue before we continued with the issues that had been assigned to us. We also shared prior knowledge especially in gitlab and its working which allowed us to all be on the same boat when it comes to saving the work that we had done using commands such as git stash among others. Also students like Anesti and Andrew who had stayed for a while since doing their software, design and architecture class were able to catch up on the structure of Thea's Pantry thanks to assistance from all the other team members.

Generally we did well, but I belive that we could do a better job in the distribution of tasks. We could have specific people work on roles that are related, example one person could specialize in tasks related to the Api, front end or backend. Also our lack of experience cost us in minor ways such as breaking down the epics into issues and also the in the process of assigning weights of issues. We were also over ambitious as we thought that we could accomplish more issues than we acutally could. Some of us ended up taking too many issues which eventually we had to return as we couldn't work on them all. I also realized that not most of us are not active and frequent users of Discord, some of the updates shared would be realized slightly before we met which led us to preferring to create a chat group instead.

Having completed the sprint short of the number of weights that we took, I expected myself to have closed more issues considering my understanding of the tasks at hand. I spent more time in class assisting my classmates rather than working on the issues that I had assigned myself. Also, I would have accomplished closing more issues if I had dedicated more time outside class to work on the issues that we had been assigned as a team. Now that I am now more familar with the structure and the working of the reporting system I expect myself to handle most of the issues that we had in the first sprint faster and more efficiently. 
