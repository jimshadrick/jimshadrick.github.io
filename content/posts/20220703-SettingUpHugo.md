---
title: "Setting Up A Site Using Hugo and GitHub Pages"
description: "My experience in setting up a static web site using Hugo and GitHub Pages"
date: 2022-07-03T20:22:23-05:00
draft: false
tags:
  - "hugo"
---

## Background
I have been wanting to setup a static website so that I could begin writing and publishing some articles on a personal blog, but I did not want to have to pay for a hosted solution. I also did not need a full featured CMS like WordPress. About two years ago I was reviewing several static website generators like Jekyll, Hugo, Gatsby, etc. and Hugo was touted as the fastest framework and seemed to be the easiest to install and setup. It appealed to me as a Windows user that it did not require Ruby or Linux or other technical dependency. It also has many themes available to choose from.

I found out pretty quickly it was easy to install and get run locally, however getting it deployed to GitHub Pages and setup a continuous build workflow was another matter. A lot of this had to do with my limited experience at the time with Git, repositories, and understanding the structure of the Hugo framework. I eventually abandoned the effort.


## Another Attempt
Fast forward to July 2022. I was coming up on a long three-day July 4 weekend and had some time available, so I thought that I would try again to get a web site up and running using Hugo and GitHub Pages. I thought that things may be different now that I knew a little more about Git, GitHub, etc., and that by having a little more knowledge, that I could have a site setup relatively quickly using GitHub Pages - a day or two at most. Boy was I wrong :frowning: 

Setting up a site and deploying it on GitHub Pages was still an undertaking. I spent over 2 days looking at article after article, downloading and trying multiple themes but each time I tried it resulted in deployment errors. A lot of this was due to the fact that these articles I was referring to were of varying levels of technical complexity, were based on different environment variables, but mostly they were all slightly different approaches. It was extremely hard to compare across the articles to gain a sense of what needed to be done to deploy the site, much less setup workflows to automatically update the site.

## Schnerring's Guide
I am a person who likes challenges. However after multiple attempts to get Hugo deployed to GitHub Pages all unsuccessful, I was just about to give up. Then I ran across this blog article ([Create a Hugo Website with GitHub Pages, GitHub Actions, and Cloudflare](https://schnerring.net/blog/create-a-hugo-website-with-github-pages-github-actions-and-cloudflare/) from [Michael Schnerring](https://twitter.com/schnerringo) which outlined in great detail everything from setting up VSCode to work with Hugo but also how to deploy the site to GitHub Pages and even automate the build process. 

From Michael's article:

> In this beginner guide, you’ll create a Hugo website from scratch and publish the website on GitHub Pages. You’ll configure Cloudflare’s DNS and utilize its caching capabilities to optimize page speeds. Finally, implementing automated deployments with GitHub Pages will enable you to publish new content on your site easily.

## End Results
There is a lot of detail that is provided in this guide, which is good but does require you to stop and understand what each step is doing. Instead of blindly typing the command lines I took the time to read the additional commentary about each step and understand the context of what was being done. This lengthened the time it took for me to complete the setup and deployment but will pay dividends down the road if I need to deploy another site.

I elected to skip the sections on setting up and connecting the site to CloudFlare, but I was able to complete all of the configuration and deployment steps using another Hugo theme [LoveIt](https://github.com/dillonzq/LoveIt). 

## Next Steps
Having gotten my site deployed to GitHub Pages successfully with my workflow running for auto-publishing, I am now spending more time understanding Hugo commands, site structure, and how to create and manage content. Once I am comfortable with this, I may explore getting a domain name, configuring the site with CloudFlare and even tailoring the look and feel with the site .css.

If you have had difficulties like I did creating and publishing a site using Hugo and GitHub Pages, I would highly recommend that you take a look at Michael Schnerring's guide. It will save you a lot of headaches in the end.

