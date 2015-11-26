---
layout: post
title: "Part 1: Introducing Couchbase Server"
description: ""
category: 
tags: []
---
{% include JB/setup %}

<h1><strong>History of Couchbase</strong></h1>
Couchbase is an open source, distributed cache, key value and JSON document database, that ships with a powerful and rich ANSI-compliant SQL language for easy developer adoption. 

It emerged out of two open source projects, Memcached and CouchDB, to address modern scalability, performance, HA and data flexibility challenges.

![Couchbase Evolution](/assets/images/couchbase-evolution.png)

Memcached is a very popular open source caching technology. However it has many inherent limitations and as a result, the original engineers of Memcached developed Membase as a drop-in replacement. 

Membase started out as an enterprise ready Caching and Key Value database and eventually evolved into Couchbase when CouchDB engineers added JSON document support. 

As a result, Couchbase is a drop-in replacement for Memcached deployments as well as a powerful key-value and document database. In one consolidated solution you get the performance benefits of a cache and the persistence guarantees of a database. 

{% highlight json %}
{
	"Couchbase addresses inherent Memcached Limitations" : [
  	{
  		"#" : 1, 
  		"problem" : "No clustering, difficult to manage individual instances",
  		"solutions" : [ "Clustered & distributed from the get-go", 
  		  		"120+ monitoring stats for easy maintance",
  		  		"Rich Web UI for easy management",
  		  		"Easy Programmatic management using REST/CLI"],
  		"solved" : true
  	},
  	{
  		"#" : 2,
  		"problem" : "Cold Cache",
  		"solutions" : [ "A consolidated Cache & Key Value database",
  		  		"Warm-up from local disk"],
  		"solved" : true
  	},
  	{
  		"#" : 3,
  		"problem" : "No high availability, crash == stampeding herd!",
  		"solutions" : [ "Built-in Replication for high availability & Disaster Recovery",
  		  		"Automatic failover"],
  		"solved" : true
  	},
  	{
  		"#" : 4,
  		"problems" : [ "Key loss during scale out (Ketama hashing)", 
  		  		"Manual code/config changes and app restarts required"],
  		"solutions" : [ "Hash based auto-sharding == even data distribution == NO hot-spots",
  		  		"100% Key availability during scale out",
  		  		"Easily scale w/o touching app code/config & w/o restarting servers"],
  		"solved" : true
  	}
 ]
}
{% endhighlight %}

Today, the original engineers of both open source technologies continue to work for Couchbase, adding cutting edge innovations and continuously improving performance and scale. 


<h1><strong>Key Couchbase Features</strong></h1>

Couchbase provides a robust foundation focused on scale, performance and high availability for mission critical applications. On top of this solid foundation, Couchbase has added powerful developer features. In a nutshell it satisfies the needs of Architects/Operations & Developers. 

1. Enterprise grade Caching, Key-Value and Document database solution
2. High availability and Disaster Recovery
	* Intelligent rack/zone aware replication
	* Auto-failover
	* Cross data center replication
4. Comprehensive monitoring stats and programmatic management via REST/CLI
5. Security
	* Encryption over the wire, 
	* On disk Encryption 
	* LDAP/AD integration, roles and auditing
6. SQL (ANSI compliant) for JSON documents
	* Reuse SQL skills to easily query documents
	* Extended SQL for JSON structures (embedded documents, collections) and flexible data models  
	* Use prepared statements and even cache query plans
	* ODBC/JDBC connectors
7. Global secondary indexes
	* Improve SQL query performance
	* Queries can use multiple indexes (intersect-scans)
	* Filters/Partial indexes using WHERE predicates
	* Covering indexes
	* Function based indexes
8. Views (distributed indexes) built using incremental map/reduce
	* Great for near realtime aggregations
	* Composite indexes for powerful view queries
	* Built in reducers for counts, sums, stats 
	* Geo-spatial & multi-dimensional indexes and queries
9. Multi-dimensional scaling
	* Scale up or out
	* KV, query & index workload isolation 
10. Hadoop, Spark, Kafka, ES/Solr connectors
11. Embedded database and Synchronization platform 
	* For offline/online mobile apps
	* Great for IOT use cases
12. Full Text indexes and scored search results (developer preview)

![Couchbase - The Complete Data Management Solution](/assets/images/couchbas-data-platform.png)

<h1><strong>The 4 principles of Couchbase</strong></h1>

Couchbase is built about 4 principles

1. <h2><strong>Consistent High Performance at Scale</strong></h2>
- A single commodity server can support hundreds of thousands of operations per second
- Sub-millisecond latency (< 1ms at the 95% percentile)
- High performance reads, writes and mixed workloads

2. <h2><strong>Easy & Affordable Scalability</strong></h2>
- Scale with a few clicks (so easy my computer illiterate mother can do it)
- Scale Linearly
- Small clusters (3 to 10 servers) can handle extremely high throughput @ <1ms latency
- Scale to billions of items

3. <h2><strong>Enterprise level High Availability and Easy Maintenance</strong></h2>
- Easily (again my mother can do it) replicate up to 3 times
- Intelligently replicate with Rack/Zone awareness, allowing for multiple server failures, even with one replica copy
- All maintenance tasks can be done with zero downtime
- Replicate an entire database(s) across multiple data-centers for Disaster recovery

4. <h2><strong>Flexible data model with Flexibly Queries</strong></h2>
- No need to define rigid schemas, change or extend schema at runtime
- JSON natively maps to application objects
- Extremely suited to agile development 
- Use SQL to flexible express queries over your flexible data structure! (No need to learn a bespoke query API)
- Full text search (developer preview)

![Couchbase - 4 Principles of Couchbase](/assets/images/4pillars.png)

In the next blog post, [Part 2: Couchbase architecture in a Nutshell](/2015/11/26/part-2-couchbase-architecture-in-a-nutshell/), we dive into the nuts & bolts of Couchbase architecture, explaining how it elegantly implements these core principles into its design.

