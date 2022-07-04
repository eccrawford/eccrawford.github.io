---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: 
permalink: /resources/
feature_image: /assets/resources2.jpg
feature_text: <h2>Resources</h2>
---

Here you'll find various teaching resources and materials for courses I've taught. As I develop more I'll likely organize it better, but for now, here are a mix of posts.

{% assign posts = site.posts | where:"type", "resources" %}

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