---
layout: default
comments: true
---
<h2>Hopefully something interesting will happen here soon.</h2>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
<iframe frameborder='0' src='https://www.indiana.edu/~oidd/feedreader/read.php?url=https://mathemaphysics.github.io/feed.xml&maxitems=0&bgcolor1=FFFFFF&bgcolor2=FFFFFF&sort=published' width='100%' height='750px'></iframe>

