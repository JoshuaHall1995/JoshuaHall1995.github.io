---
layout: page
title: Josh's Laboratory
permalink: /joshsLaboratory/
---

"In Josh's Laboratory, lives the most average boy you've ever seen!
But failing tests blow his experiments to smithereens!
There is gloom, and doom while things go boom
in Josh's Lab!"

[<img src="{{ site.baseurl }}/images/dexterLab.png" alt="Animated Josh" 
    style="width: 400px; 
    display: block;
    margin-left: auto;
    margin-right: auto;"/>]({{ site.baseurl }}/)

(Disclaimer this would have been called Josh's playgroud but that had negative connocations)

Sometimes, when the sun hits just right and the Netflix binge isnt quite hitting the spot it is time to roll out a new repo,
write to the console and have some fun creating errors I am not being paid to fix.
-----------------------------------,

{% for post in site.labratory %}

[{{ post.title }}]({{ site.baseurl }}{{ post.url }})
====================================================

{{ post.excerpt }}

[Read More]({{ site.baseurl }}{{ post.url }})

{% endfor %}