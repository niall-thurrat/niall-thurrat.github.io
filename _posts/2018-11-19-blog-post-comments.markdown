---
layout: post
title:  "How I implemented blog post comments"
author: Niall Thurrat
---

***
As you will see I have added a really nice comment functionality to the bottom of my blog posts. Anyone can do this quite easily with a blog comment hosting service and I have chosen to use Disqus.  Once I had created a free account with Disqus, I was able to register this site with them by creating a specific shortname.  I was then able to add that shortname as a reference into my _config.yml file.  My website is using the Jekyll SSG, so I needed to place an ‘if’ statement into my layout file (which is used by all my blog post files) that included my disqus comments code if the disqus shortname existed in my site. The code itself (placed in _includes/disqus_comments.html) is largely based around the disqus universal code installation instructions.  I decided to use the disqus_config variable as it defines ‘this.page.url’ and ‘this.page.identifier’ which is important for preventing duplicate threads.
***