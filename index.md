---
layout: page
---

Hi and welcome to my Github Pages.  I've generated this site as a requirement for my web programming program at Linnaeus University, so what initial content exists will be for the benefit of passing my courses. Hopefully you'll find it interesting! 

Sorry for the mandatory About Me section, my teachers forced me to write it. You'll also find a Blog Posts section with a number of posts regarding programming topics which are relevant to my program. Feel free to comment if you feel the need to do so.... I didn't add those comment boxes just to look pretty ;)

Here is a list of the separate topics in my Blog Posts page:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>