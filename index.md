---
title: Home
---
## Hello

I am Deletecat; welcome to my website! There's not much for me to say besides that I like cats (obvs!!), computers and coding.

### Recent posts
{% assign counter = 0 %}
{% for post in site.posts limit: 3 %}
- [{{post.date | date: "%d %B %Y" }} - {{post.title}}]({{post.url}}) {% if counter == 0 %}![new post](/assets/gifs/new.gif){% assign counter = 1 %}{% endif %}
{% endfor %}

### Git repository locations

I mirror my projects across several locations. Here's a list:

+ Self-hosted [soft-serve](https://github.com/charmbracelet/soft-serve): `ssh://git.deletecat.com:23231`
+ GitHub: <https://github.com/Deletecat>
+ Codeberg: <https://codeberg.org/Deletecat>

### Contact me
+ Email: [kit@deletecat.com](mailto:kit@deletecat.com)
+ XMPP: @deletecat@chat.raccoon.quest (PREFERRED)

I have accounts in other places. But if you are a stranger, those are the two that I would prefer you contact me with.

### Links
+ dpgonline: <https://dpg.deletecat.com>
+ flashcarts wiki: <https://flashcarts.net>
