---
layout: default
title: Junior Memoirs
permalink: /juniorMemoirs/
---

### Coming Soon!

Occasionally I still wake up in a hot sweat as I have flashbacks to my Advanced Programming coursework in Univercity. Sleep deprived and with a single function trying to parse a crossword that has reached over 500 lines with variables named "giveMeMercy" I awake terrified that I going to eternally be a failure and end up moving back to Snodland to drink on a street corner. 

Thankfully that did not come to pass and the years since have been much kinder. But because it is all so recent I can still picture younger Josh and I wonder what I would have told him. 

So this series shall explore the little lessons I learned to make the early stages of my career fall into place and go from a loud developer annoying everyone to a loud developer annloying everyone who gets stuff done. 

{% for post in site.juniorMem %}

[{{ post.title }}]({{ site.baseurl }}{{ post.url }})
====================================================

{{ post.excerpt }}

[Read More]({{ site.baseurl }}{{ post.url }})

{% endfor %}