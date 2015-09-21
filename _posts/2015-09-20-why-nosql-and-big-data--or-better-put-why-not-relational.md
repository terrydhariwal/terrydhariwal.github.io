---
layout: post
title: "why noSQL (and big data) ... or better put why NOT relational"
description: ""
category: "the_basics"
tags: ["noSQL basics", "big data"]
---
{% include JB/setup %}

## why noSQL

Over the past decade and a half there has been a massive increase in the demand for information in real time. This began with the dot com boom and since the invention of the smart phone and tablets the demand has grown exponentially. 

Over this period of time businesses that relied on traditional relational databases slowly began to realise the challenges posed with dealing with hundreds of thousands or even millions of operations per second, millions of concurrent connections and terabytes or even petabytes of data.

Large enterprises such as Google and Facebook quickly came to the realisation that relational databases were not suitable for many of these use-cases - which naturally gave rise to the creation of noSQL databases, big data and cloud computing. 

I will talk about the difference between the noSQL and big data in a separate blog, however think of noSQL as the operational database (OLTP) and big data as your data warehouse (OLAP) solution.

## its not about relational v noSQL
I'd like to make it clear that I'm not advocating that noSQL is a relational database replacement. Relational databases have been around for over 30 years - they are very mature and very good at what they do - ACID transactions. However it is clear that there are many use-cases that are much better suited to noSQL. These include use-cases requiring:

* ***Extremely high performance***
  * throughput - hundreds of thousands to millions of operations per second
  * latency - sub-millisecond response times
  * for read or write heavy and mixed workloads
* ***Easy and affordable linear scalability***
  * the ability to affordable and easily scale
  * supporting terabytes of data and billions of records
  * ability to intelligently scale ... scale up or scale out or both
  * scale with commodity hardware 
* ***High availability & Disaster recovery***
  * out of the box data replication and failover capabilities
  * ability to replicate across data-centres for disaster recovery
  * ability to perform maintenance without downtime
* ***Flexible data models and flexible queries***
  * the ability to handle complex data types
  * ability to hanlde date model changes in real time
  * ability to query data flexibly (for example supporting SQL)



