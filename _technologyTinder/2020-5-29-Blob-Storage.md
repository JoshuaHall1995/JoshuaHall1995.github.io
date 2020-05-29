---
layout: post
title: Blob Storage
permaLink: /2020-5-29-Blob-Storage/
---
So you want to store some data, the format be dammed? Azure Blob Storage can do that as home for unstructured data in the cloud, with data kept in directory-like structures called Containers. Unlike other NoSQL options BLOB lets you store data without a specific data model or type. Like me on Tinder, it accepts all.

<img src="{{ site.baseurl }}/images/blobTinder.png" alt="Blob storage tinder" 
    style="width: 400px;
    display: block;
    margin-left: auto;
    margin-right: auto;"/>

<h2>What is it?</h2>
As mentioned above, Azure Blob Storage is a NoSQL storage solution. Offered as one of a variety of built in Azure storage options Blob can store random Blob Storage can offer writing and reading operations for any random data type which can run at the same time and scale massively. 

This is useful for collections designed to take in thousands of records and because it was designed to be able to handle OS backups it can break large files down to reduce upload time and append changes where needed to existing blobs which can grow to multiple terabytes in size. 

<h3>Helpful Tip:</h3>
Blob does not care what you give. So if it is a file type you want to view you better specify the file type when you upload it. Usually all files are stored as an application/octet-stream by default. That means if you upload a funny picture or even a .json data file if you dont specify the type you will not be able to view the properties as expected in the portal. 

<h2>Types of Blob</h2>
When writing to blob storage there are three types of blobs you can use.  These are each designed for specific use cases. 

* Block blobs: Block blobs are composed of blocks and are ideal for storing text or binary files, and for uploading large files efficiently. Reading/writing is sped up by breaking the files into thousands of smaller blocks which can be fetched asynchronously.  Perfect for normal everyday usage.

* Page blobs: Page blobs are a collection of 512-byte pages, which provide the ability to read/write arbitrary ranges of bytes. Perfect for structures like OS and data disks for Virtual Machines and Databases

* Append Blobs: Optimised for append scenarios like log storage, Append blogs are composed of several blocks of different sizes – up to a maximum of 4 MB. Perfect for a file that shall always grow and you do not want to be overwritten by a silly developer and his love of Upsetting. 

(Thank you Microsoft for the smart wording) I butchered)

<h2>Real Life Use Case </h2>

A senior developer I was working with explained a less then compelling case for the Blob: as a happy little placeholder. 

Everywhere I have worked debates have taken place regarding the storage of the data access layer of an application and whether CosmosDB, Sql or a rucksack with the information printed off and delivered by carrier pigeon was the best option for the project. 

Inevitably the perfect solution for the problem ends up not being the one implemented. Because software is designed to be decoupled and with technologies ideally easy to switch Blob presents a less polished but scalable and cheap initial repository for a proof of concept project you can easily switch out later.  

I think this is an interesting perspective and if you have already committed to the Azure Cloud using an inbuilt data storage solution unit you know if Cosmos is correct for your scenario and wallet it is a good way to go.  Iterative improvements as infrastructure. 

<h2>Access Tiers</h2>
When you create a storage account you are able to specify the access tier. Each is designed with unique use cases in mind. 

* Hot Access Tier: Out of the three options, the hot access tier is the most optimised for data that is accessed frequently. It offers the lower access (read-write) cost, but the highest storage cost.
* Cool Access Tier: This option is better suited for use cases where data will remain stored for at least 30 days and is not accessed frequently. Compared to Hot Access Tiers,, this tier offers lower storage cost and higher access costs.
* Archive Access Tier: Archive storage is designed for data that doesn’t need to be accessed immediately. This tier offers higher data retrieval costs, and also higher data access latency. It is designed for use cases where data will be stored for more than 180 days and is rarely accessed.

<h2>Conclusion</h2>

Blob storage provides users with a storage solution that can easily be adapted to the user’s needs which is highly available and can be geo-replicated. Azure Blob Storage is a suitable all in one solution that may not be as advanced in regards to all the  No-Sql features solutions like CosmosDb can provide but as a jack of all traits it is a good option.

Perfect for a swipe until you are more sure of exactly what you want. BlobStorage likes cats and dogs, steak and vegan casserole. BlobStorage will be there until you no longer need it. 
