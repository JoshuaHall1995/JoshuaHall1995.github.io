---
layout: page
title: Junior Memoirs
permalink: /juniorMemoirs/
---

Occasionally I still wake up in a hot sweat as I have flashbacks to my Advanced Programming coursework in Univercity. Sleep deprived and with a single function trying to parse a crossword that has reached over 500 lines with variables named "giveMeMercy" I awake terrified that I going to eternally be a failure and end up moving back to Snodland to drink on a street corner. 

Thankfully that did not come to pass and the years since have been much kinder. But because it is all so recent I can still picture younger Josh and I wonder what I would have told him. 

So this series shall explore the little lessons I learned poetically recalled to a fictional younger version of myself. Who says therapy cant be free?

{% for post in site.juniorMemoirs %}

[{{ post.title }}]({{ post.url }})
====================================================

{{ post.excerpt }}

[Read More]({{ site.baseurl }}{{ post.url }})

{% endfor %}