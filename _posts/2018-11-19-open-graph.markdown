---
layout: post
title:  "What is Open Graph?"
author: Niall Thurrat
---

***
If you check out the *The Open Graph protocol* website at [http://ogp.me/](http://ogp.me/) you will read that OG 'enables any web page to become a rich object in a social graph'.  But what does that mean? To put it in simpler terms, OG means you can turn your web pages into graph objects, which will be displayed any time the URL is written in social media platforms such as Facebook or Twitter. All you need is a simple bit of code in your html tag and at least four OG meta tags in the head of your document and you're flying. When your URL is written or pasted, a box will also be displayed showing details such as the title, description and an image to represent your site.

For me using the Jekyll boilerplate, it was a little trickier. I had to copy my head.html into my _includes folder and default.html into my _layouts folder to make the changes there. It also took me a while to figure out how to make reference to the image, but a little reading on Jekyll's website about the assets folder and a bit of experimentation and it magically appeared. I used a very useful Open Graph Preview plugin for Chrome which worked on my localhost and made the whole process a lot smoother. 

***