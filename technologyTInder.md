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

<div class="posts2">{% for post2 in site.tinderTech %}

<article class="post2">

# [{{ post2.title }}]({{ site.baseurl }}{{ post2.url }})

<div class="entry">{{ post2.excerpt }}</div>

[Read More]({{ site.baseurl }}{{ post2.url }})</article>

{% endfor %}</div>