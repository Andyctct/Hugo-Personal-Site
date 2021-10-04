+++
categories = ["educational"]
comments = false
date = 2021-09-06T15:04:47-07:00
draft = false
showpagemeta = true
slug = "creating-this-website"
tags = ["personal"]
title = "How to create a website like this"
description = "My very brief journey of creating a static site with Hugo"

+++

Actual Published Date: September 21, 2021

Disclaimer: As per the description, this is going to be an extremely short and barebones guide towards setting up a site of this (low) caliber. I'm essentially just going to document the steps I took to put this website out. The guide will primarily be written with the  beginner - intermediate developer in mind.

- Step 1: The very first thing I did was do some research the different ways of building a website which include hardcoding, using a    static site generator and then deploying, or using a CMS. [This](https://theunlikelydeveloper.com/build-a-static-website/) is a good article covering the basics of what a static site is and what popular SSG options are. I chose to use a static site generator because I had never worked with one before and I thought it would be a good learning experience (and I didn't want to do too much work directly with html / css). My next goal and another option I would recommend for any beginners reading this is looking into building a website with react / vue, this is based off recommendations from friends as well as online public opinion. 

- Step 2: After deciding that I wanted to work with an SSG and picking Hugo, I moved on to learning the basics of Hugo. For learning Hugo, I believe [this](https://www.youtube.com/watch?v=qtIqKaDlqXo&list=PLLAZ4kZ9dFpOnyRlyS-liKL5ReHDcj4G3) is the best introductory hugo playlist by far as it even shows up in the gohugo documentation many, many times. 

- Step 2.5: Along with learning the fundamentals of Hugo, I think it is very useful to learn / refresh yourself on the basics of Markdown / html again. With this being my first time really working with Markdown, I had to learn it from scratch but found it really quite simple and I think taking the time to read through [this](https://daringfireball.net/projects/markdown/syntax) article will be more than enough to get you through the basics of working with Markdown.

- Step 3: Honestly, step 2 was the bulk of this short learning journey and I moved on to picking a theme from <https://themes.gohugo.io/>. From here, I encourage you to read, read, and read more documentation. If the problem you're looking for isn't solved by reading the official documentation, then try looking elsewhere on the web, you're probably studying computer science so you should be used to this by now. Next, I will list out some of the solutions I found to problems that I ran into and think might be somewhat common for beginners, and other links that I think will be useful at this stage. 
    - [Hugo website, explore it (especially the documentation)](https://gohugo.io/)
    - [Hugo shortcodes](https://gohugo.io/content-management/shortcodes/)
    - [Goa Theme Github Issues Page](https://github.com/kaapiandcode/hugo-goa/issues?page=1&q=is%3Aissue+is%3Aclosed)
    - [How to Make a Custom 404 Page in Hugo](https://stackoverflow.com/questions/53142088/how-to-make-hugo-server-use-custom-404-html)
    - [Static CSS Changes Not Updating in Hugo](https://discourse.gohugo.io/t/static-css-changes-no-updating-browser-cache-with-hugo-serve/16169)
    - [Overriding a Theme's Template and Static](https://gohugobrasil.Netlify.app/themes/customizing/)
    - [Introduction to the go Templates Hugo uses](https://gohugo.io/templates/introduction/)
    - [Understanding the dot a little better](https://www.smashingmagazine.com/2021/02/context-variables-hugo-static-site-generator/)
    - [Hugo Cheat Sheet](https://www.git-tower.com/learn/cheat-sheets/hugo/)

- Step 4: Time to deploy / host the website, this was an unexpectedly hard step for me probably because I was rusty working with git. First, it's probably a good idea to decide what you want to use to host your website because what steps you will need to take will depend on which hosting service you decide on. Popular options include Netlify, github pages, heroku, firebase, and AWS. This site is hosted on Netlify which I chose because of recommendations from friends as well as online resources, but I also thought strongly about github pages. After you choose a hosting service, you'll want to make sure that you have a remote github repository for the site if you aren't already using one for this project. For people who are completely new to this, there's a lot of documentation online about creating a github repository and the basics of working with git, I promise you it's not that bad. Once you create this repository and push your files to it (I don't believe you have to push ALL your files in order to host the website, but it's probably a good idea anyways), you can follow the steps to deploying on Netlify as written in the official Hugo documentation [here](https://gohugo.io/hosting-and-deployment/hosting-on-Netlify/). And voila, hopefully everything works out as simple as that, but as you probably know by now, that's sadly rarely the case. So here are some resources relating to problems that I ran into at this stage.
    - [Again, Hugo documentation for hosting on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-Netlify/)
    - [Deployment failing due to host key verification](https://answers.Netlify.com/t/hugo-site-deployment-failed-due-to-host-key-verification/783/4)
    - [Rules for good git commit messages](https://chris.beams.io/posts/git-commit/)
    - [CSS not loading in site](https://answers.Netlify.com/t/css-not-loading/17773/4)
    - [What the public folder is for](https://discourse.gohugo.io/t/why-is-there-a-public-folder/27979/5)
    - [How to stop hosting on Netlify](https://docs.Netlify.com/configure-builds/stop-or-activate-builds/)
    - [How to deploy using github pages](https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7)     

- Extra Steps (Optional): Now that we have deployed, there are a few other things that we can do to further improve our website. 
    - One common way forward is setting up a custom domain name which will allow us to remove the netlify.app extension of our website as well as enable us to do other things on Netlify such as enable TLS certificates (a layer of security for your website). Most likely, you will have to purchase a custom domain, but there are free options out there such as the Namecheap student pack (which only works with Github Pages I believe). Common places to purchase a domain include Google Domains, Namecheap, GoDaddy, Bluehost, etc. Then, the "Getting started" section of your site overview page on Netlify will take you through the process of setting up the domain which should be painless. 

    - Another thing we can do is integrate Netlify CMS with our existing Hugo site. For those who don't know, a CMS is a content management system and integrating it with our static site will allow us to organize and publish our content easier. I am choosing not to take this step at the moment because I want to work a little bit more with the fundamentals of Hugo for now, and I will move on to make a nicer site as my next project soon. For those who want to take this leap, it doesn't seem to me like this improvement will require vast amounts of additional learning, I believe [this](https://dev.to/howtocode_io/how-to-build-a-jamstack-blog-with-hugo-Netlify-cms-and-zapier-14dc) is a good article detailing the process. It even goes a little bit further than I mentioned, feel free to take a look if you really want to take things to the next level. 

All in all, I hope this guide was useful just to show a brief overview of the process of creating a site like this, and I hope it helps get people started on their journey of web development alongside mine.