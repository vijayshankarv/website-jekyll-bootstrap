---
layout: post
title: "How to make a webpage similar to this one"
description: ""
category: 
tags: [jekyll, website, docs]
---
{% include JB/setup %}

Writing down what I encountered while getting set up with a Jekyll bootstrap page on Github. 

I created this website following the instructions at [Jekyll Quickstart](http://jekyllbootstrap.com/usage/jekyll-quick-start.html). 
As promised in the article, I was able to get the site up and running within a couple of minutes, but I hit a few snags. 

 - The bootstrap themes were not being rendered. 
 - Jekyll serve from my local computer was throwing an error. 
 - Github emailed me saying that the pygments syntax highlighter was not supported anymore and that they were using rouge. 

### Fixing Bootstrap 
After some googling, I found that all I needed to do was to create a new bootstrap-3 directory under the assets/themes folder of my repo and move the bootstrap folder there. This was kind of a bummer since I just downloaded the git repo and got started -- turns out the git repo has not been updated in a year. 

Here is the list of commands that I used (to check how bash renders)
``` shell
cd assets/themes
mkdir bootstrap-3
mv bootstrap/ bootstrap-3/
```

### Jekyll Serve

I did not have the latest version of ruby or rubygems on my Ubuntu 16.04 machine. I followed the instructions on this page to  follow the instructions on this page and modify




### Closing thoughts
Jekyll bootstrap and github-pages is a relatively easy way to get started with building a website, if all you are looking for is a small personal blog. If your website grows, it might be time to take a look at alternatives such as [Hugo]() which may be faster 