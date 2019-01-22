---
layout: default
---
<h2>Hopefully something interesting will happen here soon.</h2>
<p>
This is an equation:
<script type="math/tex">\displaystyle f(x) = \int_0^1 g(x-y) u(y) dy</script>
</p>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

<!-- Mathjax Support -->
<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

