---
title: "Resources I used in building this website"
layout: post
date: 2021-01-13 10:47
image: /assets/images/jekyll-github.png
headerImage: true
tag:
- website
- github-pages
- jekyll-themes
star: true
category: blog
hidden: false # don't count this post in blog pagination
author: azhu513
description: Some resources I used and lessons I learned from building this website
---

At the beginning of this past Christmas break, I decided to build my personal website. This is a long overdue project, which I have been thinking of for a while but didn't have a whole block of time to really finish it. Actually, it took me only less than a day to put the information of teaching, publications, sotware and presentations into different markdowns. But I spent about two days to understand the structure of the files, what are [sass](https://sass-lang.com/guide) files, where to change headers or add navigation links etc. After building this website, I think I should write down my learning process and keep a record of the resources that I used. So if in the future I were going to build a new website, I'd come back to this post and find them easier.

I googled "how to build an academic website", and learned about [Hugo](https://gohugo.io/) and [Jekyll](https://jekyllrb.com/) from Rob William's post on [Building an Academic Website](https://jayrobwilliams.com/posts/2020/06/academic-website/). I scanned both Hugo themes and Jekyll themes, and eventually decided to use the [indigo](https://github.com/sergiokopplin/indigo) theme build by [Sérgio A. Kopplin](https://github.com/sergiokopplin) with Jekyll. 
Basically it's jekyll with Github pages. I like how it looks simple, yet have the ability to link to different pages. And I could write blogs! 

After forking the original [indigo](https://github.com/sergiokopplin/indigo) repository, I started to customize my personal website. First thing first, I followed the set up steps in the README page. Then I turned to the `_config.yml` file where I customized many elements on the home page. I found a close read of the comments in this file help clear many questions I had.

I realized that this theme does not come with a more detailed documentation for users. I found the Arti Annaswamy's post [Build a Blog with GitHub - Part 2](http://www.artiannaswamy.com/build-a-github-blog-part-2) is a good compliment to read  and an easy to follow tutorial, especially on adding pages, customizing headers, tracking traffics and adding tools for comments. One extra comment I would like to add on top of the post is that, when adding new pages, besides modification in the `header.html`, I would also recommend to add the page in the `_config.yml`. Another helpful resource by Vishal Gupta on [Creating your own site and blog with Jekyll and Markdown](http://vishalgupta.me/init/) sheds light on posting blogs.

With all the above steps, I basically have build a full website with all information I want to put on. I could have stopped here. But I also customized the color of the theme, and the font sizes. Now these changes were basically made within the `sass` files and I did a lot of trials and errors. I may post another blog giving more details about this. 

Last note is that when I build the website, I run the website locally and check if I like the layouts and stuff before I push to the git repository. [This page](https://jekyllrb.com/docs/) from Jekyll website tells very clearly how to do it.

