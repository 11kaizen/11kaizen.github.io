---
layout: post
title:  "IndependentStudy:GitKitRefactor"
date:   2023-10-02 19:00:00 -0400
categories: [CS@Worcester]
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


Over the week I began working on refactoring the Gitkit project. In the two weeks prior to this I worked alongside Prof. Karl and Dr. Stoney in developing the path I would take in refactoring the GitKit as welll as understanding the project itself. For the first sub-epic that I created [link](https://gitlab.com/groups/hfossedu/kits/-/epics/12), I intended to create a new configuration file written in YAML, the first issue within the sub-epic was to work on the merging the deploy.sh files. One on the high level directory and the other within the FarmData2 directory. After reading through the code within both files and figuring out other areas in the de that had calls I proceeded to merge the files. The build command worked and so I proceeded to commit my work thinking I had aced it in one but the problems began....

The pipeline failed due to the wrong commit message syntax as well as a failed test. After checking previous merge requests done by other collaborators in the organization, I discovered that the commit messages had to be written in a conventional manner. Luckily, I remembered the syntax that we used earlier in my Software Capstone class and after using git commit --amend the pipline succeded. However, my tests would not pass, and so I spent the rest of my time trying to learn how the testing worked.

Today in my meeting with Prof. Karl today we were able to trouble shoot the testing and we resolved by moving the features directory into the highest level of the working directory. We also discovered that we should change the naming convention of the git kit environment. I will come up with a way to append the name of the project before the kit name so that we can have GitKits follow the [project name]-kit methodology. Back to testing, we realized the importance of the gold image in testing and ended up generating a new gold image which acted as a kind of checkpoint to ensure that we have a reference point as I make adjustments to the code. As we tinkered with the testing technique it led us to discover that at some point during refactoring the project I would have to do manual testing on the project to ensure that everything works and the gold image is right. 

Overall, it was a good learning experience and a good refresher into the world of collaboration and opensource software. I hope to achieve more as the semster progresses.


