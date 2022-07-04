---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Resources
permalink: /resources/
feature_image: https://images.unsplash.com/photo-1580706483913-b6ea7db483a0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2137&q=80
feature_text: <h2>TEJ4M</h2>
---
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