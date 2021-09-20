+++
categories = ["educational"]
comments = false
date = 2021-09-06T15:04:47-07:00
draft = false
showpagemeta = true
slug = "creating-this-website"
tags = ["personal"]
title = "How to create a website like this"
description = "My very short and not at all in depth journey of creating a static site with Hugo"

+++

Actual Published Date: TBD 

Disclaimer: As per the description, this is going to be an extremely short and barebones guide towards setting up a site of this (low) caliber. I'm essentially just going to document the steps I took to put this website out.

- Step 1: The very first thing I did was do some research the different ways of building a website which include hardcoding, using a    static site generator and then deploying, or using a CMS. This is a good article covering the basics of what a static site is and what popular SSG options are, https://theunlikelydeveloper.com/build-a-static-website/. I chose to use a static site generator because I had never worked with one before and I thought it would be a good learning experience (and I didn't want to do too much work directly with html / css). My next goal and another option I would recommend for any beginners reading this is looking into building a website with react / vue, this is based off recommendations from friends as well as online public opinion. 

- Step 2: After deciding that I wanted to work with an SSG and picking Hugo, I moved on to learning the basics of Hugo. For learning Hugo, I believe [this](https://www.youtube.com/watch?v=qtIqKaDlqXo&list=PLLAZ4kZ9dFpOnyRlyS-liKL5ReHDcj4G3) is the best introductory hugo playlist by far as it even shows up in the gohugo documentation many, many times. 

- Step 2.5: Along with learning the fundamentals of Hugo, I think it is very useful to learn / refresh yourself on the basics of markdown / html again. With this being my first time really working with markdown, I had to learn it from scratch but found it really quite simple and I think taking the time to read through [this](https://daringfireball.net/projects/markdown/syntax) article will be more than enough to get you through the basics of working with markdown.

- Step 3: Honestly, step 2 was the bulk of this short learning journey and I moved on to picking a theme from <https://themes.gohugo.io/>. From here, I encourage you to read, read, and read more documentation. If the problem you're looking for isn't solved by reading the official documentation, then try looking elsewhere on the web, you're probably studying computer science so you should be used to this by now. Next, I will list out some of the solutions I found to problems that I ran into and think might be somewhat common for beginners, and other links that I think will be useful at this stage. 
    - [Hugo website, explore it (especially the documentation)](https://gohugo.io/)
    - [Hugo shortcodes](https://gohugo.io/content-management/shortcodes/)
    - [Goa Theme Github Issues Page](https://github.com/kaapiandcode/hugo-goa/issues?page=1&q=is%3Aissue+is%3Aclosed)
    - [How to Make a Custom 404 Page in Hugo](https://stackoverflow.com/questions/53142088/how-to-make-hugo-server-use-custom-404-html)
    - [Static CSS Changes Not Updating in Hugo](https://discourse.gohugo.io/t/static-css-changes-no-updating-browser-cache-with-hugo-serve/16169)
    - [Overriding a Theme's Template and Static](https://gohugobrasil.netlify.app/themes/customizing/)
    - [Introduction to the go Templates Hugo uses](https://gohugo.io/templates/introduction/)
    - [Understanding the dot a little better](https://www.smashingmagazine.com/2021/02/context-variables-hugo-static-site-generator/)
    - [Hugo Cheat Sheet](https://www.git-tower.com/learn/cheat-sheets/hugo/)

- Step 4: Time to deploy / host the website, this was an unexpectedly hard step for me probably because I was rusty working with git. First, it's probably a good idea to decide what you want to use to host your website because what steps you will need to take will depend on which hosting service you decide on. Popular options include netlify, github pages, heroku, firebase, and AWS. This site is hosted on netlify which I chose because of recommendations from friends as well as online resources, but I also thought strongly about github pages. After you choose a hosting service, you'll want to make sure that you have a remote github repository for the site if you aren't already using one for this project. For people who are completely new to this, there's a lot of documentation online about creating a github repository and the basics of working with git, I promise you it's not that bad. Once you create this repository and push your files to it (I don't believe you have to push ALL your files in order to host the website, but it's probably a good idea anyways), you can follow the steps to deploying on netlify as written in the official Hugo documentation [here](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/). And voila, hopefully everything works out as simple as that, but as you probably know by now, that's rarely the case sadly. So here are some resources relating to problems that I ran into at this stage.
    - [Again, Hugo documentation for hosting on netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/)
    - [Deployment failing due to host key verification](https://answers.netlify.com/t/hugo-site-deployment-failed-due-to-host-key-verification/783/4)
    - [Rules for good git commit messages](https://chris.beams.io/posts/git-commit/)
    - [CSS not loading in site](https://answers.netlify.com/t/css-not-loading/17773/4)
    - [What the public folder is for](https://discourse.gohugo.io/t/why-is-there-a-public-folder/27979/5)
    - [How to stop hosting on netlify](https://docs.netlify.com/configure-builds/stop-or-activate-builds/)
    - [How to deploy using github pages](https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7)     

-Step 4.5: Now that we have deployed, it's time to use a custom domain name which will enable us to do other things on netlify. To be continued.
