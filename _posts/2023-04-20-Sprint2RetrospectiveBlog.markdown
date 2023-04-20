---
layout: post
title:  "Retrospective Blog: Sprint - 2"
date:   2023-04-20 20:30:00 -0400
categories: [CS@Worcester, CS-448, Sprint-2]
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

The second sprint in my view was more efficient than the first. Because of a good understanding of how the systems worked together and the end goal of the project we were able to work smarter as a team and fasted on individual tasks. Some of the activity I did was jumping on my tima members issues to assist, [link](https://gitlab.com/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/community/-/issues/98) as well as [link2](https://gitlab.com/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/reportingapi/-/issues/15). I also worked on reviewing merge request that other team members created [link3](https://gitlab.com/LibreFoodPantry/client-solutions/theas-pantry/reportingsystem/reportingbackend/-/merge_requests/16) this among others gave me a better understanding of the reporting system and how the different parts fit in together.

Again our communication carried us through most of the sprint. The stand up meetings, chats on discord and our activity on Gitlab allowed us to make the most of the sprint. Through communication we were able to share what we had learned, which in turn helped those who were going through related challenges to come up with more ideas on how to tackle the problem at hand. Communication also allowed us to jump on others issues and assist them. At the moment I am working with Andrew on a issue that has been challenging him for a while. He was able to share the knowledge he had gained so far which helped me understand what has worked and what has not. Through collaboration we have been able to achieve much more. I also got assistance from Scott as I was working on the updating the pipeline/CI and he helped me understand more about how docker is involved in the pipeline/CI process. Finally we also worked on more issues outside class which we had agreed to do during the last retrospective. This improved our velocity greatly!

Some of the limitations we had came in while testing, specifically chai. Our unfamiliarity with chai got the better of us as we spent more time trying to understand how chai works than actually implementing what we learnt on our sub-system. Also as I had mentioned earlier, understaing how docker is involved in creating images as well as the managing the pipleine took us quite sometime as we had to learn how the tools under Libre Food Pantry are used.

We worked generally well as a team throughout the sprint. This being our second sprint I believe that we worked exceptionally well as a team. Now that we are more familiar with the system that we are working on, I believe that we can do a better job in breaking down epics into sub-epics and issues as well as weighting them. This has been a challenge initially as we did not understand how the system worked. But now I believe that we can do a better job in assigning weights to the issues. When we failed to break down the issues into its core components, it slowed us down as we had to reorganize ourselves in understanding what truly we are working on. Over weighted issues gave us a false sense of progress while under weighted issues gave us less that we had put into learning about the issue.

As an individual I believe that I could do better on my productivity and understanding. Working through the issues as soon as I got a breakthrough I would not go deeper in understanding more about the concept and how it works. All this ties to my productivity that even though I di d well, I believe that I could do better in aiding the team in achieving success in the long term.

The second sprint was very productive overall and I am glad to have gotten a hang of things especially concering scrum and how it an agile framework where you learn as you progress.
