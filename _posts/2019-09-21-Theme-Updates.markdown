---
layout: post
author: "Eric Pinter"
title:  "Theme Updates"
date:   2019-09-21 20:00:00 -0500
categories: jekyll update
---

This blog has a new template, and new styling to go along with it. You might be wondering why I chose this [particular theme](https://github.com/brianmaierjr/long-haul).
It was purely because I tried out the alternatives and ran into more difficulties setting them up correctly than this one.

![A couple of unhelpful error messages]({{site.baseurl}}/assets/images/cmdError.png)
Setting up each was easy, but this one was the easiest to port over an existing (tiny) blog to with minimal changes.
One slight downside of the new template is that whenever I change some files all of the css breaks, and the server needs to be restarted.

![Everything being broken]({{ site.baseurl }}/assets/images/broken.png)
Some other people mentioned in class that they had the same problem, but it's not a problem that would persist once this is hosted on github.
At worst it's a slight slowdown when working on the blog and nothing more.

Updating the header image (the radical data swoosh at the top of the page) was surprisingly difficult, with a couple of edits necessary in random locations in the theme's css and header file. No really, the rule is hidden [in here](https://github.com/ericpinter/csci340blog/blob/master/assets/css/style.css) somewhere, try and find it. You might think that one of the first things that a user might want to change is the generic image of a bicycle, but apparently not. But luckily, some things like the site's navigation and contact links are as easy to edit as you would expect for an abstraction tool like Jekyll.
