---
layout: post
title: "Part 1: Introducing Couchbase Server"
description: ""
category: 
tags: []
---
{% include JB/setup %}

<h1><strong>History of Couchbase</strong></h1>
Couchbase emerged out of 2 open source projects, Memcached and CouchDB.

Memcached is the world's most popular open source caching technology used in all major verticals including finance, retail, gaming and social media to name a few. The original key developers of Memcached developed Membase as an enterprise ready Caching and Key Value database. Membase addressed many inherent limitations of Memcached:

1. A consolidated Cache and Key Value database
2. Clustered and distributed from the get-go
3. Replication and Automatic High Availability
4. Autosharding and easy scalability
5. Disk persistence


![Couchbase Evolution](/assets/images/couchbase-evolution.png)

Membase then evolved into Couchbase by introducing JSON document support. Again, like Memcached, the original developers of CouchDB were responsible for adding JSON document support. Today, the original engineers of both open source technologies continue to work for Couchbase, adding cutting edge innovations and continously improving performance and scale. 

<h1><strong>Key Couchbase Features</strong></h1>

1. An enterprise Caching, Key Value and Document database solution
2. Replication, Ultra high availability (Rack/Zone awareness)
3. Cross data center replication for Disaster recovery
4. ANSI Compliant SQL for JSON documents
5. Geo Spatial Queries
6. Distributed Indexes (Views) and Global secondary indexes
7. Embedded database and Synchronisation platform for offline/online and IOT usecases
8. Full Text Search (developer preview)

![Couchbase - The Complete Data Management Solution](/assets/images/couchbas-data-platform.png)

Its worth point out that Couchbase is now a completely distinct codebase from Memcached and CouchDB. 


<h1><strong>The 4 principles of Couchbase</strong></h1>

Couchbase is built about 4 priciples

1. <h2><strong>Consistent High Performance at Scale</strong></h2>
- A single commodity server can support hundreds of thousands of operations per second
- Sub-millisecond latency (< 1ms at the 95% percentile)
- High performance reads, writes and mixed workloads

2. <h2><strong>Easy & Affordable Scalability</strong></h2>
- Scale with a few clicks (so easy my computer illiterate mother can do it)
- Scale Linearly
- Small clusters (3 to 10 servers) can handle extremely high throughput @ <1ms latency
- Scale to billions of items

3. <h2><strong>Enterprise level High Availability and Easy Maintence</strong></h2>
- Easily (again my mother can do it) replicate up to 3 times
- Intelligently replicate with Rack/Zone awareness, allowing for multiple server failures, even with one replica copy
- All maintenance tasks can be done with zero downtime
- Replicate an entire database(s) across multiple data-centres for Disaster recovery

4. <h2><strong>Flexible data model with Flexibly Queries</strong></h2>
- No need to define rigid schemas, change or extend schema at runtime
- JSON nativily maps to application objects
- Extremely suited to agile development 
- Use SQL to flexible express queries over your flexible data structure! (No need to learn a beskpoke query API)
- Full text search (developer preview)

![Couchbase - 4 Principles of Couchbase](/assets/images/4pillars.png)

In the next blog post, [Part 2: Couchbase architecture in a Nutshell](/2015/11/26/part-2-couchbase-architecture-in-a-nutshell/), we dive into the nuts & bolts of Couchbase architecture, explaining how it elegantly implements these core principles into its design.

