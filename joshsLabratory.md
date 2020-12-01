---
layout: page
title: Josh's Laboratory
permalink: /joshsLaboratory/
---
<p style="text-align:center">"In Josh's Laboratory, lives the most average boy you've ever seen! <br>
But failing tests blow his experiments to smithereens! <br>
There is gloom, and doom while things go boom <br>
in Josh's Lab!" </p>

[<img src="{{ site.baseurl }}/images/dexterLab.jpeg" alt="Animated Josh" 
    style="width: 400px; 
    display: block;
    margin-left: auto;
    margin-right: auto;"/>]({{ site.baseurl }}/)

<h6 style="text-align:center">(Disclaimer: This would have been called Josh's playground but that had negative connotations)</h6>

Sometimes, when the sun hits just right and the Netflix binge isnt quite hitting the spot it is time to roll out a new repo,
write to the console and have some fun creating errors I am not being paid to fix.

-----------------------------------

{% for post in site.labratory %}

[{{ post.title }}]({{ site.baseurl }}{{ post.url }})
====================================================

{{ post.excerpt }}

[Read More]({{ site.baseurl }}{{ post.url }})

{% endfor %}