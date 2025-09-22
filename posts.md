---
title: Posts
---
## Post archive
{% assign counter = 0 %}
{% for post in site.posts %}
- [{{post.date | date: "%d %B %Y" }} - {{post.title}}]({{post.url}}) {% if counter == 0 %}![new post](/assets/gifs/new.gif){% assign counter = 1 %}{% endif %}
{% endfor %}
