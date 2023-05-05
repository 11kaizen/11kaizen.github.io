---
layout: post
title:  "Retrospective Blog: Sprint - 3"
date:   2023-04-20 23:00:00 -0400
categories: [CS@Worcester, CS-448, Sprint-3]
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

## Retrospect
The third and final sprint was much shorter than the first two sprints, however it is in this sprint that I achieved more that I could have expected. I worked on one issue that seemed to be more involving than I would have expected. On this issue I jumped on to help out Andrew Lam who had been experiencing some challenges on with Chai testing. [link](https://gitlab.com/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/reportingbackend/-/issues/50) I also assisted in validating some merge requests that had been created and assisting in closing issues [link2](https://gitlab.com/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/reportingapi/-/issues/10). These are some of the activities that I did on Gitlab during the course of the sprint

Something that worked really well during this sprint was the collaboration that took place. We all joined hands in the sprint to overcome the challenge that had been facing us with Chai. It was only shortly after that we realized that the Chai test were functional and correct and that it was the server that had an issue. We all joined hands and collaborated and scanned through the code and the file systems that we had and it was long after that we were able to get our server back up and running. That took us quite sometime and finally we got the test to validate correctly what the calls were requesting. Also our determination and focus to overcome the challange was something that worked really well. We utilized Discord and met outside class times inorder to make progress with the Chai issue.

I think that we would have done a better job as a team in understanding the role of the reporting system. Over the course of the two earlier sprints we got used to the idea of copy and pasting what was in the GuestInfo System. I believe this caught up to us when the server did not start up. To my realization, most of the critical files for the reporting system had been deleted and I had to go back into previous commits in order to retrive this files. We should have been more keen on understanding the function of the system in order to avoid removing the files that were important. This would also have been caught at the review stage as we validate a merge request but it also slipped through that filter.

Overall we did well as a team. Since the sprint was for a shorter duration and we had become more well versed with the system, there were no major challenges that we faced as a team. Our scrum master did a great job and we also communicated challenges that we were facing and jumped on to assist each other where need be. It has been a great experience working with the team this far and I have really leanrt how to work with agile in a team and work with a team in agile. I couldn't have asked for a better team.

One thing that I could make better about myself is teaching others what I have been able to learn. Learning how to document how I was able to solve a task or complete an issue is something that I think will be beneficial not only to me but others as well. By documenting what I have learnt others might be able to learn some troubleshooting skills such as using breakpoints with debuggin tools. For others, it might be a light bulb that might allow them to break through the bug that they are facing. This is one thing that I think working on will allow help others in their programming tasks. 
