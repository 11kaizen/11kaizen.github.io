---
layout: post
title:  "IndependentStudy:GitKitRefactor5"
date:   2023-11-23 22:00:00 -0400
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

Almost at the finish line!

We were able to achieve four to the five steps within the epic. Step 2 and 3 were very closely related and I managed to do them within one step. Creating the ordered list in config.yaml file allowed us to determine the order in which the features are installed rather than depending on the numbers that were prefixedin the indvidual feature files.


The final step, splitting the GitKit repository into KitDeploy and GitKit, is where I am at and it is quite challenging.

I decided to clone the GitKit into my on personal profile by making a repository, KitDeployTrial. KitDeployTrial would contain the eventual file structure that I would have in KitDeploy. After successfully doing this I came across a major roadblock which would not allow me to create new docker images as the pipeline structure had to be setup within the repository.

So I decided to abandon KitDeployTrial and create a new KitDeploy repository within HFOSSedu so that full functionality may be possible with the pipeline. I then moved the necessary files into the repository and the pipeline worked. I then pushed the changes to the GitKit repository but realized that the pipeline was not updating the image in the container repository.

With Professor Stoney's and Professor Karl's help I was able to understand how images worked and used the docker pull command to manually update the local image. I was therefore able to update the KitDeploy image locally and begun working on changing deploy.sh 
