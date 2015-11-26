---
layout: post
title: "Couchbase Server - Core Principles in a Nutshell"
description: ""
category: 
tags: []
---
{% include JB/setup %}

## Couchbase in a Nutshell
This 10-part blog provides the core principles of Couchbase server in bite-size pieces.
For a deep-dive I recommend reading our [online documentation](http://developer.couchbase.com/guides-and-references). 
However if you want a fast-track understanding of Couchbase - then this is the place for you.

### [Part 1: Introducing Couchbase Server](/2015/11/26/part-1-introducing-couchbase-server/)
* History of Couchbase
* The 4 pillars of Couchbase
* Key features

### [Part 2: Couchbase architecture in a Nutshell](/2015/11/26/part-2-couchbase-architecture-in-a-nutshell/)
* Single Node Architecture
* Multi-Dimensional scaling
* An introduction to the the cluster Map

### [Part 3: The Data Service - KV ops, Data Distribution and Scaling](/2015/11/26/part-3-the-data-service---kv-ops-data-distribution-and-scaling/)
* KV operations, replication and persistence
* How data is distributed and accessed
* How scale out works
* Simple KV examples

### [Part 4: A quick detour - CAP theorem](/2015/11/26/part-4-a-quick-detour---cap-theorem/)
* An introduction to CAP theorem
* CP by default. Consistency w/o sacrificing performance
* AP architecture - Cross Data Centre Replication

### [Part 5: The Data Service - Data Replication and High Availability](/2015/11/26/part-5-the-data-service---data-replication-and-high-availability/)
* Replication and Rack Zone Awareness
* How Failover works
* Automatic failover or manual
* Simple KV examples for handling failover

### [Part 6: The Data Service - Views in a Nutshell](/2015/11/26/part-6-the-data-service---views-in-a-nutshell/)
* Views (distributed indexes)
* View creation (Map Reduce) and View queries (scatter gather)
* Simple view examples

### [Part 7: The Index Service in a Nutshell](/2015/11/26/part-7-the-index-service-in-a-nutshell/)
* Multi-dimensional scaling revisited
* Index Service Architecture
* Differences between views and indexes
* A simple index example

### [Part 8: The Query Service in a Nutshell](/2015/11/26/part-8-the-query-service-in-a-nutshell/)
* Multi-dimensional scaling revisited
* Query Service Architecture
* Some simple N1QL queries

### [Part 9: KV v Views v N1QL](/2015/11/26/part-9-kv-v-views-v-n1ql/)
* Differences between KV, Views and N1QL
* 90/10 rule
* Cache your queries

### [Part 10: Disaster Recovery - Cross Data Centre Replication](/2015/11/27/part-10-disaster-recovery---cross-data-centre-replication/)
* An introduction to XDCR 
* A simple XDCR example 
* XDCR Topologies
* AP considerations