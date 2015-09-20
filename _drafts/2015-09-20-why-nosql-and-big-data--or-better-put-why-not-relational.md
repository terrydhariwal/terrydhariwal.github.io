---
layout: post
title: "why noSQL (and big data) ... or better put why NOT relational"
description: ""
category: 
tags: []
---
{% include JB/setup %}

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

One of the key weakenesses of relation database is the lack of schema flexibility
* Relational databases have rigid schemas
  * this makes it very difficult for developers working in an agile development environment

* impedence mismatch for developers
One of the key weaknesses of noSQL databases is the lack of ACID transactions across multiple records

PICTURE OF SCALEUP VS SCALE OUT


## noSQL & big data 

Sometimes these two industries are conflated however they fundamentally come from two different standpoints and address problems. 

NoSQL databases such as Couchbase, MongoDB and Cassandra address the challenges related to the real time access of operational data at extremely high throughput and extremely low sub millisecond response times. Big data technologies such as a Hadoop or Spark address the challenges of processing and analysing large quantities of data in batch or near real time. Both technologies need to handle the challenges related to unstructured or semi structured data. 

Think of noSQL as the OLTP (online transaction processing) or the operation database and big data as the OLAP (online analytical processing) or data warehouse database technology. 

It's worth noting that both seem to be converging towards operational and analytical use cases, however as always (in my opinion) not every problem is a nail and not every solution is a hammer. Thats is to say noSQL and big data strongly complement each other, so use them both when it makes sense.

Use noSQL where you need to perform 100's K's to millions of operations per second in millisecond response times and use big data when you need to process huge quantities of data to support your business processes. For example AOL, Criteo, PayPal and LivePerson to name a few use Couchbase with Hadoop/Storm/Spark. Couchbase is used to ingest vast quantities of event data and the big data technologies process this data in batch or near reatime, the output of which is stored in Couchbase to provide millisecond access for real time personalisation (next best ads) or intelligent business triggers.


