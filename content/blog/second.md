+++
categories = ["educational"]
comments = false
date = 2021-09-21T15:04:47-07:00
draft = false
showpagemeta = true
slug = "creating-this-website"
tags = ["personal"]
title = "How to create a website like this"
description = "My very brief journey of creating a static site with Hugo"

+++

Disclaimer: This is an extremely short and barebones guide towards setting up a site like this. The guide is written with the beginner - intermediate developer in mind.

- Step 1: The first thing I did was research the different ways of building a website which include hardcoding, using a static site generator and then deploying, or using a CMS. [This](https://theunlikelydeveloper.com/build-a-static-website/) is a good article covering the basics of what a static site is and what popular SSG options are. I chose to use a static site generator because I had never worked with one before and I thought it would be a good learning experience (and I didn't want to do too much work directly with html / css). My next goal and another option I would recommend for any beginners reading this is looking into building a website with react / vue, this is based off recommendations from friends as well as online public opinion.

- Step 2: After deciding that I wanted to work with an SSG and picking Hugo, I moved on to learning the basics of Hugo. For learning Hugo, I believe [this](https://www.youtube.com/watch?v=qtIqKaDlqXo&list=PLLAZ4kZ9dFpOnyRlyS-liKL5ReHDcj4G3) is the best introductory hugo playlist by far as it even shows up in the gohugo documentation many times.

- Step 2.5: Along with learning Hugo fundamentals, I think it is useful to learn / refresh yourself on the basics of Markdown / html again. This was my first time working extensively with Markdown, and I found it simple enough to learn. Taking the time to read through [this](https://daringfireball.net/projects/markdown/syntax) article should be enough to get you through the basics of working with Markdown.

- Step 3: Step 2 was the bulk of this short learning journey and I then moved on to picking a theme from <https://themes.gohugo.io/>. At this point, most of the work involves reading more and more documentation. If the problem you're looking for isn't solved by reading the official documentation, then try looking elsewhere on the web (you're probably studying computer science so you should be used to this by now). Here are some of the solutions I found to problems that I ran into, and other links that I think will be useful at this stage.
  - [Hugo website, explore it (especially the documentation)](https://gohugo.io/)
  - [Hugo shortcodes](https://gohugo.io/content-management/shortcodes/)
  - [Goa Theme Github Issues Page](https://github.com/kaapiandcode/hugo-goa/issues?page=1&q=is%3Aissue+is%3Aclosed)
  - [How to Make a Custom 404 Page in Hugo](https://stackoverflow.com/questions/53142088/how-to-make-hugo-server-use-custom-404-html)
  - [Static CSS Changes Not Updating in Hugo](https://discourse.gohugo.io/t/static-css-changes-no-updating-browser-cache-with-hugo-serve/16169)    - [Overriding a Theme's Template and Static](https://gohugobrasil.Netlify.app/themes/customizing/)
  - [Introduction to the go Templates Hugo uses](https://gohugo.io/templates/introduction/)
  - [Understanding the dot a little better](https://www.smashingmagazine.com/2021/02/context-variables-hugo-static-site-generator/)
  - [Hugo Cheat Sheet](https://www.git-tower.com/learn/cheat-sheets/hugo/)

- Step 4: Now it is time to deploy / host the website, an unexpectedly hard step for me because of my rust with git. First, you need to decide what you want to use to host your website. Popular options include Netlify, github pages, heroku, firebase, and AWS. This site is hosted on Netlify which I chose because of peer recommendations as well as online resources. After you choose a hosting service, make sure that you have a remote github repository for the site if you aren't already using one for this project. For people completely new to this, there's a lot of documentation online about creating a github repository and the basics of working with git. Once you create this repository and push your files to it (check the theme example site to see the minimum files you need to push), you can follow the steps to deploying on Netlify as written in the official Hugo documentation [here](https://gohugo.io/hosting-and-deployment/hosting-on-Netlify/). Here are some resources relating to problems that I ran into at this stage.
  - [Again, Hugo documentation for hosting on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-Netlify/)
  - [Deployment failing due to host key verification](https://answers.Netlify.com/t/hugo-site-deployment-failed-due-to-host-key-verification/783/4)
  - [Rules for good git commit messages](https://chris.beams.io/posts/git-commit/)
  - [CSS not loading in site](https://answers.Netlify.com/t/css-not-loading/17773/4)
  - [What the public folder is for](https://discourse.gohugo.io/t/why-is-there-a-public-folder/27979/5)
  - [How to stop hosting on Netlify](https://docs.Netlify.com/configure-builds/stop-or-activate-builds/)
  - [How to deploy using github pages](https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7)
  - [No URL found for submodule path in .gitmodules](https://answers.netlify.com/t/error-checking-out-submodules-fatal-no-url-found-for-submodule-path-website-in-gitmodules/16435/8)
  - [Specifying Hugo config file](https://gohugo.io/getting-started/configuration/)
  - [Hugo version not updating in Netlify](https://docs.netlify.com/frameworks/hugo/)

  - Extra Steps (Optional): Now that we have deployed, there are a few other things that we can do to further improve our website.
  - One way forward is setting up a custom domain name which will allow us to remove the netlify.app extension of our website as well as enable us to do other things on Netlify such as enable TLS certificates (a layer of security for your website). Most likely, you will have to purchase a custom domain, but there are free options out there such as the Namecheap student pack (which only works with Github Pages I believe). Common places to purchase a domain include Google Domains, Namecheap, GoDaddy, Bluehost, etc. Then, the "Getting started" section of your site overview page on Netlify will take you through the process of setting up the domain which should be painless.

  - Another thing we can do is integrate Netlify CMS with our existing Hugo site. A CMS is a content management system and integrating it with our static site will allow us to organize and publish our content easier. I have not done this yet because I want to work a little bit more with the fundamentals of Hugo for now. For those who want to take this leap, it doesn't seem to me like this improvement will require vast amounts of additional learning, I believe [this](https://dev.to/howtocode_io/how-to-build-a-jamstack-blog-with-hugo-netlify-cms-and-zapier-14dc) is a good article detailing the process.

All in all, I hope this guide was useful in showing a brief overview of how to create a site like this.
