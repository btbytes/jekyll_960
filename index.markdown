---
layout: default
title: Home
markdown: maruku
---
Welcome to your [Jekyll](http://jekyllrb.com) + [960.gs](http://960.gs) powered web site.

To start with edit the `_config.yml` and change the default `author`, `url` and `email` fields to 
to your own.

Next, add a text file under `_posts`, say `2010-01-24-hello-world.html` and run `jekyll`. The blog post
should show up below.


{% if site.posts.len > 0 %}
<section>

<h1>Blog Posts</h1>
  <ul class=posts>
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</section>

{% endif %}
