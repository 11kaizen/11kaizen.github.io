---
layout: post
title:  "IndependentStudy:GitKitRefactor4"
date:   2023-11-02 22:00:00 -0400
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

This week I was able to make more progress in refactoring the Git Kit.

I was able to separate kit specific features from general features and I also managed to have deploy.sh read the features from the config.yaml file. Both of these while maintaining functiona
lity of the kit which I tested by deploying on git hub.

When it came to separating kit specific features from general features, I created a new folder to contain the kit specific features in the top-level directory. Afterward changes were made to
 the deploy.sh so that it could look for the kit specific features in the kit specific directory rather than the general features directory. After making these adjustments, I deployed the git kit on GitHub and it worked successfully.

Having deploy.sh read the ordered list from the config.yaml file was slightly more challenging. After figuring out the order into which the features are installed, I replicated the same order in the config.yaml file. I separated them based on which function name. The next step was figuring out how yq reads the ordered list. After researching I figured out I could bring the ordered list as an array, I then created a for loop to iterate through the file names and then install the features through the deploy.sh file. After a couple of hours figuring out all this I tested the new structure and it worked!

It was a successful week, and I am glad that I continue to make progress in refactoring Git Kit.

