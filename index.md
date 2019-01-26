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

