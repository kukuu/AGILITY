
# Structured & non-Structured Databases

These are the two main types of databases in industry.

## Structured DB

Structured data refers to any data that resides in a fixed field within a record or file. This includes data contained in relational databases and spreadsheets. 

Examples: 

```

1. MySQL
2. PostgreSQL

```

### Features

i. Data Types

ii. Data Integrity

iii. Concurrency, Performance

v. Reliability, Disaster Recovery

vi. Security

vii. Extensibility

viii. Internationalisation, Text Search


## NoSQL

A NoSQL database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases. They are increasingly used in big data and real-time web applications. 

NoSQL systems are distributed, non-relational databases designed for large-scale data storage and for massively-parallel, high-performance data processing across a large number of commodity servers. They arose out of a need for agility, performance, and scale, and can support a wide set of use cases, including exploratory and predictive analytics in real-time (social media use case). They arose out of a need for agility, performance, and scale, and can support a wide set of :

 Examples: 

```

1. MongoDB

2. Casandra

3. CoucDB

```



### MongoDB

MongoDB  is a cross-platform document-oriented  NoSQL database. Classified as a NoSQL database, MongoDB eschews the traditional table-based relational database structure in favour of JSON-like documents with dynamic schemas (MongoDB calls the format BSON), making the integration of data in certain types of applications easier and faster.


#### Main features MongoDB

Some of the features include:


i. Document-oriented

    Instead of taking a business subject and breaking it up into multiple relational structures, 
    MongoDB can store the business subject in the minimal number of documents. For example, instead 
    of storing title and author information in two distinct relational structures, title, author, 
    and other title-related information can all be stored in a single document called Book, which 
    is much more intuitive and usually easier to work with.[5]

ii. Ad hoc queries

    MongoDB supports search by field, range queries, regular expression searches. Queries can return
    specific fields of documents and also include user-defined JavaScript functions.

iii. Indexing

    Any field in a MongoDB document can be indexed (indices in MongoDB are conceptually similar 
    to those in RDBMSes). Secondary indices are also available.

iv. Replication

    MongoDB provides high availability with replica sets. A replica set consists of two or more copies of 
    the data. 
    Each replica set member may act in the role of primary or secondary replica at any time. The primary
    replica performs all writes and reads by default. Secondary replicas maintain a copy of the data on 
    the primary using built-in replication. When a primary replica fails, the replica set automatically 
    conducts an election process to determine which secondary should become the primary. Secondaries can 
    also perform read operations, but the data is eventually consistent by default.

vi  Load balancing

    MongoDB scales horizontally using sharding. The user chooses a shard key, which determines how the data in a
    collection will be distributed. The data is split into ranges (based on the shard key) and distributed across 
    multiple shards. (A shard is a master with one or more slaves.)

    MongoDB can run over multiple servers, balancing the load and/or duplicating data to keep the system up and 
    running in case of hardware failure. Automatic configuration is easy to deploy, and new machines can be 
    added to a running database.

vii. File storage

    MongoDB can be used as a file system, taking advantage of load balancing and data replication features 
    over multiple machines for storing files.

    This function, called GridFS,is included with MongoDB drivers and available with no difficulty.
    GridFS is used, for example, in plugins for NGINX[9] and lighttpd.[10] Instead of storing a 
    file in a single document, GridFS divides a file into parts, or chunks, and stores each of those 
    chunks as a separate document.

    In a multi-machine MongoDB system, files can be distributed and copied multiple times between 
    machines transparently, thus effectively creating a load-balanced and fault-tolerant system.

viii. Aggregation

      MapReduce can be used for batch processing of data and aggregation operations. 
      The aggregation framework enables users to obtain the kind of results for which the 
      SQL GROUP BY clause is used.

ix. Server-side JavaScript execution

    JavaScript can be used in queries, aggregation functions (such as MapReduce), and sent directly 
    to the database to be executed.

x. Capped collections

    MongoDB supports fixed-size collections called capped collections. This type of collection maintains 
    insertion order and, once the specified size has been reached, behaves like a circular queue. 


## SQL and no-SQL : Differences, Pros and Cons and Use Cases


1. SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database. ... 

2. SQL databases have predefined schema  - which means the structure of the data should be known in advance to ensure that the data adheres to the schema. For example, predefined schema based applications that use SQL include Payroll Management System, Order Processing and Flight Reservations.(This is a better use case of SQL), whereas NoSQL databases have dynamic schema for unstructured data. RDBMSs that use SQL are schema–oriented 

3.  Built by top internet companies to keep pace with the data deluge, NoSQL data base scales horizontally, and is designed to scale to hundreds of millions and even billions of users doing updates as well as reads.

Horizontal scaling means that you scale by adding more machines into your pool of resources whereas Vertical scaling means that you scale by adding more power (CPU, RAM) to an existing machine.


4. One of the key differentiator is that NoSQL supported by column oriented databases where RDBMS is row oriented database.

5. NoSQL seems to work better on both unstructured and unrelated data. The better solutions are the crossover databases that have elements of both NoSQL and SQL.


6. SQL Databases are vertically scalable – this means that they can only be scaled by enhancing the horse power of the implementation hardware, thereby making it a costly deal for processing large batches of data.

7. Agile processing - NoSQL databases give up some features of the traditional databases for speed and horizontal scalability (JOIN and TRANSACTIONS). 

8. NoSQL databases on the other hand are perceived to be cheaper, faster and safer to extend a preexisting program to do a new job than to implement something from scratch.

9. Even though SQL has its own set of limits, it is also a very mature technology, which is well understood, and has a large pool of developers who understand how to use it well.

10. Security (Data Integrity) - More importantly, data Integrity is a key feature of SQL based databases. This means, ensuring the data is validated across all the tables and there’s no duplicate, unrelated or unauthorized data inserted in the system.

11. Working with complex querriees - Advantages of SQL databases are that they are typically more performant when dealing with more complex queries. Users cite the relational nature of SQL DBs encourages a well-structured database

Most banking institutions have a SQL-type database system



## USE CASES of using NoSQL

1. Relational databases like MySQL, PostgreSQL and SQLite3 represent and store data in tables and rows. They're based on a branch of algebraic set theory known as relational algebra. Meanwhile, non-relational databases like MongoDB represent data in collections of JSON documents.

2. NoSQL technology is mainly developed for handing unstructured data - Big Data. 

3. Addressing security
 
 RDBMSs that use SQL are schema–oriented which means the structure of the data should be known in advance to ensure that the data adheres to the schema - Right for mitigating security and data integrity. eg. Payrole and Flight Management.

4. Which is best and scales better

 SQL RDBMS are ill-suited for changing business requirements, as schema changes are problematic and time-consuming, insufficient performance (too low) and latency (too high) for the new requirements.

5. Limited ability to scale cost-effectively, if at all.

That explains the soaring popularity of NoSQL database systems that sprang up alongside major Internet companies such as Google, Yahoo and Amazon. Each had challenges in dealing with huge quantities of data in real-time, something that conventional RDBMS solutions could not cope with.


## Which is better for Analysis - SQL or NoSQL?


This depends on a lot of factors, for example the type of data one is analyzing, how much data one has and how quickly you need it. For example, for applications such as user behavior analysis, relational DB is best.

Well, if the data fits into a spreadsheet, then it is better suited for a SQL-type database such as PostGres, BigQuery as relational databases are good at analyzing data in rows and columns.

For semi-structured data, think social media, texts or geographical data which requires large amount of text mining or image processing, NoSQL type database such as mongoDB, CouchDB works best. Since running analytics on semi-structured data requires a heavy coding background, analyzing these type of DBs require a data scientist.  

When it comes to size of data, PostGres MySQL usually gives a good performance for under 1terabyte of data Amazon Redshift is preferred for petabyte scale. And with smaller teams of engineers focused on building pipelines, relational DBs take less to manage than NoSQL.

On the other hand, relational databases, one can use SQL to query them. SQL as a language is well-known among data analysts and engineers and is also easy to learn than most programming languages.


## Is NoSQL faster than SQL?

1. NoSQL seems to work better on both unstructured and unrelated data. The better solutions are the crossover databases that have elements of both NoSQL and SQL. RDBMSs that use SQL are schema–oriented which means the structure of the data should be known in advance to ensure that the data adheres to the schema.

2. MongoDB is more fast and scalable in comparison of SQL server. MongoDB doesn't support JOIN and Global transactions but SQL server supports it. MongoDB supports a big amount of data but MS SQL server doesn't.


A transaction is a logical unit of work that contains one or more SQL statements. It is an transaction is an atomic unit. The effects of all the SQL statements in a transaction can be either all committed (applied to the database) or all rolled back (undone from the database).


When a transaction is commited (COMMIT), the transaction is written to the transaction log in RAM. When a CHECKPOINT occurs (after some time and/or some transactions and other criterias), the transactions between the last CHECKPOINT and the current are written to disk

12. Is MongoDB faster than MySQL?

One single main benefit it has over MySQL is its ability to handle large unstructured data. It is magically faster.The increased  performance is  mainly because it allows users to query in a different manner that is more sensitive and directly related to the document.

A query statement directly refers to the document you are fetching.


## Resources:

https://www.youtube.com/watch?v=OrNUnlB4AmQ (1)
https://www.youtube.com/watch?v=2ajlfURobd8 (2)
https://www.youtube.com/watch?v=h1hLeGMdBv4
http://www.learn-with-video-tutorials.com



