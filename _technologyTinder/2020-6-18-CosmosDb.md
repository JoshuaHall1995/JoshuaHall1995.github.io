---
layout: post
title: CosmosDb
permaLink: /2020-6-18-CosmosDb/
---
So, everyone has preferences and built in completely random prejudices. I am not a bad person for refusing to swipe right on a person who puts, soy milk, in their likes section. For that same logic I am not a bad person for wanting to hate Cosmos from first hearing about it. SQL will always be my first. But you can always be won over. 

<img src="{{ site.baseurl }}/images/cosmos.png" alt="Cosmos tinder" 
    style="width: 400px;
    display: block;
    margin-left: auto;
    margin-right: auto;"/>

<h2>What is it?</h2>
So CosmosDb is a highly scalable NoSql database which is globally distributed. “It is a highly available, highly reliable, and high throughput database” and basically when I first read about it the sales pitch was stronger than the kind of home insurance that offers you a free meerkat plushy. 

[<img src="{{ site.baseurl }}/images/meerkat.jpeg" alt="Meerkat" 
    style="width: 400px; 
    display: block;
    margin-left: auto;
    margin-right: auto;"/>]({{ site.baseurl }}/)

But realistically the sales pitch has merit. Hooked up to the Azure cloud land you are given a storage option which can scale up with ease if suddenly needed, can be integrated with SDK’s in multiple languages and if it does fall over it is supported by Microsoft’s own services for high availability.

(You can also have your data stored to multiple consistency levels but that is for another day.)

For a place to store your non-relational data, whether you have a million requests a minute or five, CosmosDb is an option which will adapt to your needs.

Like a vegetarian who can go vegan or pescatarian depending on what you feel. Perfect for date night. 

<h2>How it looks</h2>
In regards to the structure of a CosmosDb it looks a lot like a database. Shocking. With a container representing a database and a collection akin to a table it is quite straightforward. The biggest difference is a collection has no predefined format (aside from a portion key which can be whatever you choose it to be) which means you can put any structure within reason into it. 

Like me as a kid told to clean my room, I can shove my toys next to the ugly polo shirt my mum got me for Christmas. CosmosDb does not care. 

(Bonus point: because of the multi-language support and variety of SDK’s available you can still use SQL formatted queries if you are so included to search over a Cosmos collection. Like saying “no my ex never did it like that” but they don’t decapitate you with a saucepan.)

<h2>Scalability</h2>
So, lets talk scale and how it works. It is basically the trump card of the CosmosDb dating profile, basically the “I have a dog” move. Instant swipe. 

Scalability is based on how CosmosDb stores their documents. Each document has a partition key. This is used to put similar documents into their own logical partitions. Like boxing up your possessions when you move house, you put all the kitchen items in boxes labelled “kitchen” so you don’t accidentally unpack it later in the bathroom. 

To expand this example, if you are storing boxes as objects in your collection with the partition key “kitchen” then, all boxes that are filed under kitchen will be placed in their own logical partition, others which belong to bathroom will be stored in different logical partition.

These logical partitions are stored on physical partitions. If both “kitchen” and “bathroom”  fit in the same physical portion they are stored together and all is good.

If the collection grows when you find more boxes in the shed and they reach your physical limit, CosmosDb divides the boxes out again across multiple physical locations so they can fit. 

Like putting one box in your mates car because you ran out of room.

Basically because of this scale is infinite. 

<h2>Cost</h2>
CosmosDb can be a cheap date or a wine and dine depending on how you setup your data storage. As someone who likes messing with Azure cloud integrated API’s to kill some hours but who is also terrified of dipping accidentally into their overdraft the pricing structure of cosmos scares me. And not just because RU pricing is a bit baffling.

I won’t pretend to be an expert. Basically the way CosmosDb is designed to adapt to your needs means it is also going to adapt on the bill. Scallops costs more than a Caesar salad (pescatarian throw back). 

From what I can tell cosmosDb is perfect both efficiency wise (with good latency) for collections which expect to have frequent transactions. If you plan on having a collection with only a few records the model is not as cost effective.

But as the person who has spent £10 before to get a friend's girlfriend to punch him in the junk I am not one to pretend to be an expert on cost effectiveness.

Just highlights it is not a quick fix or the cheapest option, arguably good to know what your demands are expected to be before you commit yourself. 

<h2>Cosmos vs SQL</h2>
So the elegant I the room, or more so the ex. I may be deciding whether to swipe for CosmosDb but I still have SQL on the brain. Those inner joins just can’t be beat.

On a serious level the two realistically should not be compared, they have two different use cases. SQL Server handles requests sequentially because it’s s designed with data consistency in mind. Cosmos is all about speed, eventually consistent but not always. 

CosmosDb will take whatever you throw at it, there does not need to be a consistent format beyond the partition key. SQL is much stricter. Know your use case.

CosmosDb will never be the quiet, reserved type no matter how hard you try to change it.

<h2>Conclusion</h2>
I love SQL. Not because of anything special it offers but because it was the first database solution I used and I remember, horrifically, having to manually run one stored procedure after another during a specified one-hour deployment time with no roll back strategy in a previous role (who needs automation?). 

But just because SQL holds a special place in my heart does not mean I can be closed off from all other options. CosmosDb is a fantastic solution for highly transactions systems. 

If I am looking for a SQL clone CosmosDb is not the one, it will never treat me the same way. But I have grown and changed, and as long as my requirements have as well, CosmosDb is perfect to swipe right on. 