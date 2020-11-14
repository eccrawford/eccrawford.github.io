---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Blog
permalink: /blog/
feature_image: /assets/blogbanner.png
feature_text: <h2>Blog Posts</h2>
site.categories: blog
---

{% assign posts = site.posts | where:"type", "blog" %}

<ul class="list  list--posts">
{% for post in posts %}
<li class="item  item--post">
<article class="article  article--post">
		<div class="blogpost">
        <h3 class="title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <small class="small post-meta">{{ post.date | date: "%b %d %Y" }}</small>
        {% if post.summary %}
            <p class="entry">{{ post.summary }}</p>
         {% endif %}
         </div>
 </article>
</li>
{% endfor %}
</ul>

