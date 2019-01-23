---
layout: default
title: Archive
---

# Archive

Find a specific post here, to see all the posts in one place [click here](all.md), you can also [download the archive][dl] for offline view.

{% for post in site.posts %}

<div>
  {{ post.date | date: "%b %-d, %Y" }}
    »
  <span class='post-title'>
    <a href="{{ site.path }}{{ post.url }}">{{ post.title }}</a>
  </span>
</div>

{% endfor %}

[dl]: https://github.com/alex-esc/posts/archive/master.zip