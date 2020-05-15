---
layout: page
title: Technology Tinder
permalink: /technologyTinder/
---

### Coming Soon!

Like many people my age my righ thumb has seen some action swiping for company. It is amazing how little there is interesting about you
when it is condensed down to a few hundred characters. This series of posts will be a collection of brief descriptions of different
technologies and concepts I try to come to grips with using the most basic of verbage. 

Hopefully after a read some of these will get a match, I know all to well the pain of zero connections.

<div class="posts">
  {% for post in site.posts.tinder %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>