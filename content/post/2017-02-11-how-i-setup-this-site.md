---
title: How I Setup This Site
author: John Goldin
date: '2017-02-11'
categories: []
tags: []
Categories:
  - Development
  - GoLang
Description: ''
Tags:
  - Development
  - golang
menu: main
---
I attended the **blogdown** session at the RStudio conference in Florida. I am enjoying the enthusiasm and energy around R and RStudio.
It reminds me of the early days of personal computers at the end of the 70's and the beginning of the 80's. Perhaps I am experiencing a second
childhood. Anyway, all the Cool Kids are doing web pages on GitHub so I want to do it too.

I have done some simple blog posts with Blogger and WordPress. One of my goals is to create a portfolio of the my R projects.
RMarkdown is the obvious way to go and WordPress doesn't directly support
that. So that's a motivation to use **blogdown**. But really a bit part of the
motivation is that these days I am "all in" with the RStudio set of
tools so it's natural to put my faith in Yihui Xie and jump in. Because **blogdown** is still developing,
I know I am goint to suffer through rough edges. As a retiree, I am
doing this for fun so the rough edges just add to the adventure.

### GitHub Pages
I had a little trouble to start because I didn't understand the basics of
what was going on with GitHub and web pages. Here I am focused on what GitHub refers to as a "user site" (as opposed to an organization site or a project site). See their [general description of GitHub Pages](https://pages.github.com/) and [What is GitHub Pages?](https://help.github.com/articles/what-is-github-pages). The key
fact is that if you have a repository called `username.github.io` (with your
GitHub username), whatever is in that repository will be served
as a web site accessed as `https://username.github.io`. What
we are going to do here is describe how to use **markdown**, RStudio,
and GitHub to place the content of a static web site into
your `username.github.io` repository.

### GitHub
The site relies on **blogdown** and GitHub. You have to have at least a beginner's familiarity with GitHub, and believe me, I am merely a
GitHub beginner. I got my start with GitHub mostly based on information
from Jenny Bryan (see [Happy Git and GitHub for the useR](http://happygitwithr.com/)) and from [RStudio](https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN). There's also an [introduction](https://guides.github.com/activities/hello-world/) on the GitHub site.

You need to be able to create a repository on GitHub and then
clone that to a project in RStudio. See especially [section 16](http://happygitwithr.com/new-github-first.html) on Happy Git.

In general I try to operate in a way that allows me to rely on RStudio to do most of the work and to avoid doing git commands in the Terminal on OSX.
That's why I create a minimal repository first on GitHub and then create
a new project in RStudio that clones the repository from GitHub. Rely on
Jenny's directions on how to do that.

### Creating a website
To get started with blogdown, I relied on a post by [Amber Thomas](https://proquestionasker.github.io/blog/Making_Site/),
especially the comments on the post by Yihui Xie, the creator of
**blogdown**. Amber's instructions involve more work with Git than I wanted
to attempt. In particular, she uses multiple branches. Instead,
I followed the suggestion and created two repositories.
One was for the site itself (`johngoldin.github.io`) and the other (which I called `pages-source`) contains the **blogdown** and **Hugo** material
that actually produces the site. 

1. Create a repository for username.github.io on your github.
2. Clone that to a RStudio project with the same name.
3. Create a repository on your github, any name you desire, but here we will calle it `hugo-source`.
4. Clone that second project to an RStudio project.

You are going to use **blogdown** to create a **Hugo** site in
`hugo-source`. And you are going to configure that site
so that whenever it builds a website, it will place that
website into the RStudio project username.github.io.
When you push username.github.io to GitHub you will in effect
publish your website.

(Actually it doesn't matter whether or not you maintain
a GitHub repository for `hugo-source`. It depends on whether
you want to use version control for convenience or backup, just
as would be true for any other RStudio project.)

