---
layout: post
title: "what is noSQL"
description: ""
category: 
tags: []
---
{% include JB/setup %}

## so what is noSQL?

NoSQL encompasses a wide variety of database technologies, that were specifically developed in response to:

<ol type='a'>
<li>an extreme rise in data volumes (web-scale), </li> 
<li>coupled with the need for extremely high performance reads and writes (web-performance) </li>
<li>the need to handle complex and agile (flexible) data models</li> 
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
The following are common characteristics that noSQL databases strive for. Note not all noSQL databases exhibit these characteristics:

* store denormalised data as apposed to normalised (relational)
* trade-off complex joins (relational) and ACID transactions for greater scalability and performance
* designed for horizontal and online scaling
* designed for commodity hardware 
* they strive for flexible data schemas as apposed to rigid schemas in relational databases. NoSQL databases can handle complex data model changes in realtime without downtime
* they are designed for high availability - through the use of data replication and auto-healing
* they tend to be distributed database technologies - they are therefore subject to CAP theorem (more on this in later blogs). 

In the next blog I drill into why noSQL exists and when to use noSQL versus when to use relational.
