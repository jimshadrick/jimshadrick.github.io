---
title: "Building a website powered by Hugo and GitHub Pages"
description: "My experience in setting up a static web site using Hugo and GitHub Pages"
date: 2022-12-03T20:22:23-05:00
draft: false
tags:
  - "hugo"
---

## Background

I have been wanting to setup a static website so that I could begin writing and publishing some articles on a personal blog, but I did not want to have to pay for a hosted solution. I also did not need a full featured CMS like WordPress so began looking at several static website generators like Jekyll, Hugo, Gatsby, etc. Hugo was touted as the fastest framework and seemed to be the easiest to install and setup with less dependencies. There were also has many themes available to choose from compared with the other frameworks.

Although I am not a developer by trade, I found out pretty quickly it was easy to install and get run locally. However getting it deployed to GitHub Pages and setup a continuous build workflow was another matter. A lot of this had to do with my limited experience at the time with Git, repositories, and understanding the structure of the Hugo framework. More on this later ...

## First Steps

My first steps were pretty straightforward which were to install Hugo locally.

- https://gohugo.io/getting-started

Because I am running Windows 11, I used the Scoop package manager to install Hugo:

`scoop install hugo-extended`

## Prepared GitHub

From my GitHub account I created a new repository with a user type named **jimshadrick.github.io** and initialized it with a `README` and `LICENSE` file. You can find out more about GitHub Pages and setting up sites in the [GitHub Docs](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#types-of-github-pages-sites)

## Remaining Steps

As part of my research into Hugo and GitHub Pages, I ran across this excellent article ([Create a Hugo Website with GitHub Pages, GitHub Actions, and Cloudflare](https://schnerring.net/blog/create-a-hugo-website-with-github-pages-github-actions-and-cloudflare/) from [Michael Schnerring](https://twitter.com/schnerringo) which outlined in great detail everything from setting up VSCode to work with Hugo but also how to deploy the site to GitHub Pages and even automate the build process.

Rather than repeat all of those steps which are outlined in this article, here were the remaining high level steps I performed:

- Clone the newly created GitHub Pages repository
- Open the repository in VSCode (my preferred editor of choice)
- Install some VSCode extensions to aid in content and editing the site
- Add a .gitignore file for the development environment and Hugo artifacts
- Push the development environment settings to GitHub
- Create a new site using Hugo in the workspace
- Add the [LoveIt theme](https://hugoloveit.com/theme-documentation-basics/)
  `git submodule add https://github.com/dillonzq/LoveIt.git themes/LoveIt`
- Update the theme configuration
- Add some content and test running the site locally
- Push the changes to GitHub
- Deploy the site to GitHub Pages
- Automate future deployments with GitHub Actions

There is a lot of detail that is provided in this guide, which is good but does require you to stop and understand what each step is doing. Instead of blindly typing the command lines I would recommend you take the time to read the additional commentary about each step and understand the context of what was being done. This lengthened the time it took for me to complete the setup and deployment really helped in my overall understanding of the site structure and mechanics.

Note: I elected to skip the sections on setting up and connecting the site to CloudFlare.

## Summary

Having gotten my site deployed to GitHub Pages successfully with my workflow running for auto-deployments, I am now spending more time understanding Hugo commands, site structure, and how to create and manage content. Once I am comfortable with this, I may explore getting a domain name, configuring the site with CloudFlare and even tailoring the look and feel with the site .css.

Hopefully this information is helpful for anyone like thinking about setting up your own static website on GitHub Pages.
