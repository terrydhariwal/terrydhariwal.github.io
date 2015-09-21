---
layout: post
title: "noSQL & big data"
description: ""
category: "the_basics"
tags: ["noSQL","big data"]
---
{% include JB/setup %}

## noSQL & big data

NoSQL & big data technologies have emerged to address performance and scalability issues faced by relational databases due the following web-based mega-trends:

* an exponentional rise of data volumes (BIG DATA)
* a huge rise in concurrent users - handling 100'000's to millions of read/writes per second (BIG USERS)
* the need to handle complex and flexible data structures in agile development environments (FLEXIBLE DATA)
* the rise of cloud computing has lowered the barriers for SME's to compete with established technology giants (CLOUD COMPUTING) 

![web mega trends](/assets/images/mega_trends.png)
![big data trends](/assets/images/big_data_trends.png)
[Source: IDC 2011 Digital Universe Study](http://www.emc.com/collateral/demos/microsites/emc-digital-universe-2011/index.htm)


Sometimes these two industries are conflated however they fundamentally come from two different standpoints and address different problems.

NoSQL databases such as Couchbase, MongoDB and Cassandra address the challenges related to the real time access of operational data at extremely high throughput and extremely low sub millisecond response times. These databases support real time web applications that need to perform low latency CRUD operations.  

Big data technologies such as a Hadoop or Spark address the challenges of processing and analysing large quantities of data in batch or near real time. The key difference between noSQL and big data is the fact that big data solutions tend to read and process every record in the warehouse, whereas noSQL tends to focus on sparse queries on individual records. 

Both technologies need to handle the challenges related to unstructured or semi structured data.

Think of noSQL as the OLTP (online transaction processing) database and big data as the OLAP (online analytical processing) or data warehouse database technology.

![Real Time Big Data](/assets/images/nosql_and_big_data.png)

It's worth noting that both seem to be converging towards operational and analytical use cases, however as always (in my opinion) not every problem is a nail and not every solution is a hammer. Thats is to say noSQL and big data strongly complement each other, so use them both when it makes sense.

For example AOL, Criteo, PayPal and LivePerson to name a few, use Couchbase with Hadoop/Storm/Spark:

* Couchbase is used to ingest vast quantities of event data at high velocity throughput 
* and the big data technologies process this data in batch or near reatime, 
* the output of which is stored in Couchbase to provide millisecond access for real time personalisation (next best ads) or intelligent business triggers.


