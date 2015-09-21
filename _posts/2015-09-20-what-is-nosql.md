---
layout: post
title: "what is noSQL"
description: "what is noSQL all about?"
category: "the_basics" 
tags: ["noSQL basics","big data"]
---
{% include JB/setup %}

## so what is noSQL?

NoSQL encompasses a wide variety of database technologies, that were specifically developed in response to:

<ol type='a'>
 <li>an exponential increase in data volumes (web-scale), </li>
 <li>a huge rise in concurrent end-users as a result of smart phones/devices</li> 
 <li>the need to handle extremely high performance reads and writes (web-performance) </li>
 <li>the need to handle complex and agile (flexible) data models</li>
 <li>the increased demand for "always on" applications - high availability and disaster recovery</li> 
</ol>

Relational databases on the other hand were not designed to cope with web scale and web-performance applications. They particularly struggle with agile or flexible data models.

## what does noSQL stand for?
There are many arguments about the meaning of noSQL. Initially it was an acronym for "no SQL" but it has evolved to mean "not only SQL" or non-relational. For instance Couchbase is an open source document database that supports SQL queries.

## types of noSQL
There are many categories of noSQL databases. The key types are:

* Caching 
* Key Value
* Document
* Columnar 
* Graph
* Full text search

I <del>have explained</del> will explain each style of noSQL database in another blog. 

## common noSQL characteristics
The following are common characteristics that noSQL databases strive for. Note not all noSQL databases exhibit all of these characteristics:

* data tends to map very closely to application objects
  * the data model tends to be inferred from the application tier
  * data is much more denormalised as apposed to normalised (relational)
  * there is less or no impedence mismatch between application and database data models
  * there is a trade-off of expensive/complex joins (relational) and ACID transactions for greater scalability and performance
  * most noSQL databases can handle simple and very complex data structures 
  * JSON based document databases can handle:
    * strings, numbers, booleans and datetimes 
    * support composite or embedded documents 
    * support collections of simple or complex data types
* flexible data models as apposed to rigid schemas (in relational). 
  * records belonging to the same data type (equivalent to a table in relational) have a common data structure (infererred from app tier) 
  * however these entities can have a varying number of values in collections and can also be extended to have additional properties or attributes 
  * denormalised & flexible data models allow noSQL to update an individual record's data model in realtime without downtime and without impacting every other record.
* horizontally and online scalablebility
  * designed to run on commodity hardware
  * designed to scale while online (without code changes and application/database downtime)
* high performance reads and writes 
* high availability and disaster recovery ootb 
  * LAN & WAN replication and auto-healing
  * distributed database technologies (they are therefore subject to CAP theorem - more on this in later blogs. 

In the next blog I drill into why noSQL exists and when to use noSQL versus when to use relational.
