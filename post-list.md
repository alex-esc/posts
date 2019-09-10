---
layout: default
title: Blog posts in reverse chronological order
redirect_from:
- /allposts.html
- /postlist.html
- /listpost.html
- /postslist.html
- /listposts.html
- /allblogposts.html
- /blogpostslist.html
- /blogpostlist.html
---


{% for post in site.posts %}

<div>
  {{ post.date | date: "%b %-d, %Y" }}
    »
  <span class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">{{ post.title }}</a>
  </span>
</div>

{% endfor %}