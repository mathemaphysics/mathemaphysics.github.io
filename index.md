---
layout: default
comments: true
---
<h2>Latest Posts</h2>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

<h2>Recent Progress</h2>
<blockquote class="trello-card"><a href="https://trello.com/c/ULG2wi9l/1-combine-python-binance-and-coinbase-apis">Combine Python Binance and Coinbase APIs</a></blockquote><script src="https://p.trellocdn.com/embed.min.js"></script>


