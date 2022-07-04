---
title: "Setting Up A Site Using Hugo and GitHub Pages"
description: "My experience in setting up a static web site using Hugo and GitHub Pages"
date: 2022-07-03T20:22:23-05:00
draft: false
tags:
  - "hugo"
---

## Background
I have been wanting to setup a static website to begin writing some articles, but I did not want to have to pay for a hosted solution nor did I need a full featured CMS like WordPress. About two years ago I had tried to use Hugo and was able to get a site up and running locally. However when it came to deploying it to a web hosting service like GitHub Pages or Netlify, the blogs and articles I read seemed so overwhelming and my attempts were all met with failure. A lot of this had to do with my limited experience with Git, repositories, and understanding the structure of the Hugo framework.


## One More Try
Given I was coming up on a long three-day July 4 weekend, I thought that I would give it another go. I thought that things may be different and that I could get a site setup relatively quickly using GitHub Pages in a day or two at most. Boy was I wrong. Setting up a site and deploying it on GitHub Pages has been a long slog. I spent over 2 days looking at article after article, downloading and trying multiple themes but each time I tried it resulted in deployment errors. A lot of this was due to the fact that these articles I was referring to were of varying levels of complexity or were based on different environment variables, the author's technical knowledge and experience, as well as different approaches. It was extremely hard to compare across the articles to gain a sense of what needed to be done to deploy the site, much less setup workflows to automatically update the site.

## Schnerring To The Rescue
I am a person who likes challenges. Even though my background has been in finance, I have taught myself C# and .Net concepts and a little bit of Javascript. In learning some of these new languages and tools I have never shied away from a challenge. However after multiple attempts to get Hugo deployed to GitHub Pages, I was just about to give up. Then I ran across this blog article ([Create a Hugo Website with GitHub Pages, GitHub Actions, and Cloudflare](https://schnerring.net/blog/create-a-hugo-website-with-github-pages-github-actions-and-cloudflare/) from [Michael Schnerring](https://twitter.com/schnerringo) which outlined in great detail everything from setting up VSCode to work with Hugo but also how to deploy the site to GitHub Pages and even automate the build process. 

From Michael's article:

> In this beginner guide, you’ll create a Hugo website from scratch and publish the website on GitHub Pages. You’ll configure Cloudflare’s DNS and utilize its caching capabilities to optimize page speeds. Finally, implementing automated deployments with GitHub Pages will enable you to publish new content on your site easily.

## Wow, It Worked!
There is a lot of detail that is provided in this guide, which is good but does require you to stop and understand what each step is doing. Instead of blindly typing the command lines I took the time to read the additional commentary about each step and understand the context of what was being done. This lengthened the time it took for me to complete the setup and deployment but will pay dividends down the road if I need to deploy another site.

I elected to skip the sections on setting up and connecting the site to CloudFlare, but I was able to complete all of the configuration and deployment using another Hugo theme [LoveIt](https://github.com/dillonzq/LoveIt).

Now I need to spend some more time with Hugo to understand the content structure and how to tailor the site to my preferences. 

