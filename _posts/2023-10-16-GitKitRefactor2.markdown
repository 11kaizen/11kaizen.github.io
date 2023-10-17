---
layout: post
title:  "IndependentStudy:GitKitRefactor2"
date:   2023-10-16 22:00:00 -0400
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

Hit the first major obstacle in the project.

In my previous blog I had indicated that I would begin manually testing the GitKit by deploying it on Github. The first step was to look for the corresponding container to deploy from the registry. The professor he showed me exactly where the container was, it was tagged by my branch name. A new container is always generated when the pipeline is built with the same tag as the branch name.

At this is point is where I hit the roadblock. After trying to deploy the container I experienced errors. Considering the changes that I had made in trying to merge the deploy.sh files, I realized that I had started off on the wrong foot. I needed to start again, I needed a clean slate. After more retrys of deploying the container I realized that I had to make the tough choice of starting all over again. I deleted my branch and deleted the local files. I created a new branch.
  
A fresh start.
  
Rather than using the local test on the GitKit repository, I decided that a successful deploy on GitHub would by my means of testing. I immediately got to testing the new branch I created without making any changes, which worked. I then proceeded to merge deploy.sh, after careful evaluation I realized that the only important variable in the high level deploy.sh was KIT_PROJECT_PREFIX which I redefined in the FarmData2/deploy.sh. I commented out the original deploy.sh and pushed the changes.
  
I tested. It worked.

The next step I decided would be to begin working on the yaml file that would contain the configurations of the GitKit. After looking at the link that Prof. Stoney had recommended, I learnt how to use yq, a command line YAML processor, and implemented it in deploy.sh [export TARGET_ORG="${yq '.TARGET_ORGANIZATION' config.yaml}"]. After multiple tries to deploy the Git Kit I kept on running in to an error. I tried manipulating deploy.sh in various ways but it was unsuccessful. It wasn't until I met with the professor that I realized that I had been trying to configure the wrong variable. TARGET_REPO,TARGET_COMMIT were the variables that I was to include in the configuration file. And after trying it worked! 

I also managed to cut down the testing time by reducing the number of labels and issues being created in the JSON files under the features directory.

Despite it being a challenging, journey I feel like I am generally getting to understand the Git Kit system and making progress in refactoring it. The next step is now to move deploy.sh into the top-level directory as I progressively move the features directory to the top-level.

"Furthermore, it is an honors project" - Its going to be challenging
