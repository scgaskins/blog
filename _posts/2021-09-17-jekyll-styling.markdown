---
layout: post
title:  "Jekyll Styling"
author: Sammy
---
Working through this lab, I found Jekyll to be pretty easy to use. Overriding the theme defaults works pretty intuitively. Though I don't understand the Ruby code in the theme files well enough to alter it, I feel that I could pretty easily alter any of the HTML.

I continued to learn how to work with Markdown in modifying my [about page](/blog/about/) and in creating my [cats page](/blog/cats/). It took me a bit of work to figure out how to link to different pages within my blog. At first, I thought I could just use the permalink, for example `/about/` for the about page. I needed several tries to realize that every internal link needed to start with `/blog/`.

I was a bit frustrated that the markdown syntax for adding images doesn't allow resizing the image. For example, this picture of my cat Peaches comes out far too big when inserted in the default way of `![Peaches](/blog/Images/Peaches.JPG)`.

![Peaches](/blog/Images/Peaches.JPG)

I need to use the HTML code

    <img src="/blog/Images/Peaches.JPG" alt="Peaches" width=<width>>

to control its width.

<img src="/blog/Images/Peaches.JPG" alt="Peaches" width=400>
