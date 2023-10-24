---
layout: post
title:  "IndependentStudy:GitKitRefactor3"
date:   2023-10-23 22:00:00 -0400
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

I am making progress!

Last week's fresh start prooved to be more beneficial than I expected.

It made this week's progress much easier. I was able to move deploy.sh to the top level directory which worked well after testing by deploying the FarmData2 GitKit on GitHub. After this worked I also moved the features directory to the top level directory and after minor changes in the deploy.sh file in the pre-install-features and install-features functions, I got it working. It was a huge step.

Having completed these tasks I am now complete with the first step within the epic that we had created.

I also managed to update the gold.raw image that is used in testing, as well as reinstating the original json files that were within the the features 6 and 7 directory. Finally I squashed all my inital commits into a single commit which has a message stating that i completed the first step in the epic.

The next step will now go deeper into separating the git kit specific feautes from the general features. Heading into some choppy waters!

New Lesson learned in scripting:
$(...) ${...}.
Parens are command substitution. Curlies are variable substitution. 
 
