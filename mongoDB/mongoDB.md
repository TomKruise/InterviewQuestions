# MongoDB Interview Questions

### 1) What do you understand by NoSQL databases? Is MongoDB a NoSQL database? explain.

At the present time, the internet is loaded with big data, big users, big complexity etc. and also becoming more complex day by day. NoSQL is answer of all these problems, It is not a traditional database management system, not even a relational database management system (RDBMS). NoSQL stands for "Not Only SQL". NoSQL is a type of database that can handle and sort all type of unstructured, messy and complicated data. It is just a new way to think about the database.

Yes. MongoDB is a NoSQL database.

---

### 2) Which are the different languages supported by MongoDB?

MonggoDB provides official driver support for C, C++, C#, Java, Node.js, Perl, PHP, Python, Ruby, Scala, Go and Erlang.

You can use MongoDB with any of the above languages. There are some other community supported drivers too but the above mentioned ones are officially provided by MongoDB.

---

### 3) What are the different types of NoSQL databases? Give some example.

NoSQL database can be classified as 4 basic types:

1. Key value store NoSQL database
2. Document store NoSQL database
3. Column store NoSQL database
4. Graph base NoSQL databse

There are many NoSQL databases. MongoDB, Cassandra, CouchBD, Hypertable, Redis, Riak, Neo4j, HBASE, Couchbase, MemcacheDB, Voldemort, RevenDB etc. are the examples of NoSQL databases.

---

### 4) Is MongoDB better than other SQL databases? If yes then how?

MongoDB is better than other SQL databases because it allows a highly flexible and scalable document structure.

**For example:**

* One data document in MongoDB can have five columns and the other one in the same collection can have ten columns.
* MongoDB database are faster than SQL databases due to efficient indexing and storage techniques.

---

### 5) What type of DBMS is MongoDB?

MongoDB is a document oriented DBMS

---

### 6) What is the difference between MongoDB and MySQL?

Although MongoDB and MySQL both are free and open source databases, there is a lot of difference between them in the term of data representation, relationship, transaction, querying data, schema design and definition, performance speed, normalization and many more. To compare MySQL with MongoDB is like a comparison between Relational and Non-relational databases.

---

### 7) Why MongoDB is known as best NoSQL database?

MongoDb is the best NoSQL database because, it is:

Document Oriented

Rich Query language

High Performance

Highly Available

Easily Scalable

---

### 8) Does MongoDB support primary-key, foreign-key relationship?

No. By Default, MongoDB doesn't support primary key-foreign key relationship.

---

### 9) Can you achieve primary key - foreign key relationships in MongoDB?

We can achieve primary key-foreign key relationship by embedding one document inside another. For example: An address document can be embedded inside customer document.

---

### 10) Does MongoDB need a lot of RAM? 

No. There is no need a lot of RAM to run MongoDB. It can be run even on a small amount of RAM because it dynamically allocates and de-allocates RAM according to the requirement of the processes.

---

### 11) Explain the structure of ObjectID in MongoDB.

ObjectID is a 12-byte BSON type. These are:

* 4 bytes value representing seconds
* 3 byte machine identifier
* 2 byte process id
* 3 byte counter

---

### 12) Is it true that MongoDB uses BSON to represent document structure?

Yes.

---

### 13) What are Indexes in MongoDB?

In MondoDB, Indexes are used to execute query efficiently. Without indexes, MongoDB must perform a collection scan, i.e. scan every document in a collection, to select those documents that match the query statement. If an appropriate index exists for a query, MongoDB can use the index to limit the number of documents it must inspect.

---

### 14) By default, which index is created by MongoDB for every collection?

By default, the_id collection is created for every collection by MongoDB.

---

### 15) What is a Namespace in MongoDB?

Namespace is a concatenation of the database name and the collection name. Collection, in which MongoDB stores BSON objects.

---

### 16) Can journaling features be used to perform safe hot backups?

Yes.

---

### 17) Why does Profiler use in MongoDB?

MongoDB uses a database profiler to perform characteristics of each operation against the database. You can use a profiler to find queries and write operations

---

### 18) If you remove an object attribute, is it deleted from the database?

Yes, it be. Remove the attribute and then re-save() the object.

---

### 19) In which language MongoDB is written?

MongoDB is written and implemented in C++.

---

### 20) Does MongoDB need a lot space of Random Access Memory (RAM)?

No. MongoDB can be run on small free space of RAM.

---

### 21) What language you can use with MongoDB?

MongoDB client drivers supports all the popular programming languages so there is no issue of language, you can use any language that you want.

---

### 22) Does MongoDB database have tables for storing records?

No. Instead of tables, MongoDB uses "Collections" to store data. 

---

---

### 23) Do the MongoDB databases have schema?

Yes. MongoDB databases have dynamic schema. There is no need to define the structure to create collections.

---

### 24) What is the method to configure the cache size in MongoDB?

MongoDB's cache is not configurable. Actually MongoDb uses all the free spaces on the system automatically by way of memory mapped files.

---

### 25) How to do Transaction/locking in MongoDB?

MongoDB doesn't use traditional locking or complex transaction with Rollback. MongoDB is designed to be light weighted, fast and predictable to its performance. It keeps transaction support simple to enhance performance.

---

### 26) Why 32 bit version of MongoDB are not preferred ?

Because MongoDB uses memory mapped files so when you run a 32-bit build of MongoDB, the total storage size of server is 2 GB. But when you run a 64-bit build of MongoDB, this provides virtually unlimited storage size. So 64-bit is preferred over 32-bit.

---

### 27) Is it possible to remove old files in the moveChunk directory?

Yes, These files can be deleted once the operations are done because these files are made as backups during normal shard balancing operation. This is a manual cleanup process and necessary to free up space.

---

### 28) What will have to do if a shard is down or slow and you do a query?

If a shard is down and you even do query then your query will be returned with an error unless you set a partial query option. But if a shard is slow them Mongos will wait for them till response.

---

### 29)Explain the covered query in MongoDB.

A query is called covered query if satisfies the following two conditions:

* The fields used in the query are part of an index used in the query.
* The fields returned in the results are in the same index.

---

### 30) What is the importance of covered query?

Covered query makes the execution of the query faster because indexes are stored in RAM or sequentially located on disk. It makes the execution of the query faster.

Covered query makes the fields are covered in the index itself, MongoDB can match the query condition as well as return the result fields using the same index without looking inside the documents.

---

### 31) What is sharding in MongoDB?

In MongoDB, Sharding is a procedure of storing data records across multiple machines. It is a MongoDB approach to meet the demands of data growth. It creates horizontal partition of data in a database or search engine. Each partition is referred as shard or database shard.

---

### 32) What is replica set in MongoDB?

A replica can be specified as a group of mongo instances that host the same data set. In a replica set, one node is primary, and another is secondary. All data is replicated from primary to secondary nodes.

---

### 33) What is primary and secondary replica set in MongoDB?

In MongoDB, primary nodes are the node that can accept write. These are also known as master nodes. The replication in MongoDB is single master so, only one node can accept write operations at a time.

Secondary nodes are known as slave nodes. These are read only nodes that replicate from the primary. 

---

### 34) By default, which replica sets are used to write data?

By default, MongoDB writes data only to the primary replica set.

---

### 35) What is CRUD in MongoDB?

MongoDB supports following CRUD operations:

* Create
* Read
* Update
* Delete

---

### 36) In which format MongoDB represents document structure?

MongoDB uses BSON to represent document structures.

---

### 37) What will happen when you remove a document from database in MongoDB? Does MongoDB remove it from disk?

Yes. If you remove a document from database, MongoDB will remove it from disk too.

---

### 38) Why are MongoDB data files large in size?

MongoDB doesn't follow file system fragmentation and pre allocates data files to reserve space while setting up the server. That's why MongoDB data files are large in size.

---

### 39) What is a storage engine in MongoDB?

A storage engine is the part of a database that is used to manage how data is stored on disk.

**For example:** one storage engine might offer better performance for read-heavy workloads, and another might support a higher-throughput for write operations.

---

### 40) Which are the storage engines used by MongoDB?

MMAPv1 and WiredTiger are two storage engine used by MongoDB.

---

### 41) What is the usage of profiler in MongoDB?

A database profiler is used to collect data about MongoDB write operations, cursors, database commands on a running mongod instance. You can enable profiling on a per-database or per-instance basis.

The database profiler writes all the data it collects to the system. profile collection, which is a capped collection.

---

### 42) Is it possible to configure the cache size for MMAPv1 in MongoDB?

No. it is not possible to configure the cache size for MMAPv1 because MMAPv1 does not allow configuring the cache size.

---

### 43) How to configure the cache size for WiredTiger in MongoDB?

For the WiredTiger storage engine, you can specify the maximum size of the cache that WiredTiger will use for all data. This can be done using storage.wiredTiger.engineConfig.cacheSizeGB option.

---

### 44) How does MongoDB provide concurrency?

MongoDB uses reader-writer locks for concurrency. Reader-writer locks allow concurrent readers shared access to a resource, such as a database or collection, but give exclusive access to a single write operation.

---

### 45) What is the difference between MongoDB and Redis database?

**Difference between MongoDB and Redis:**

* Redis is faster than MongoDB.
* Redis has a key-value storage whereas MongoDB has a document type storage.
* Redis is hard to code but MongoDB is easy.

For more information: [click here](https://www.javatpoint.com/redis-vs-mongodb)

---

### 46) What is the difference between MongoDB and CouchDB?

**Difference between MongoDB and CouchDB:**

* MongoDB is faster than CouchDB while CouchDB is safer than MongoDB.
* Triggers are not available in MongoDB while triggers are available in CouchDB.
* MongoDB serializes JSON data to BSON while CouchDB doesn't store data in JSON format.

For more information: [click here](https://www.javatpoint.com/couchdb-vs-mongodb)

---

### 47) What is the difference between MongoDB and Cassandra?

**Difference between MongoDB and Cassandra:**

* MongoDB is cross-platform document-oriented database system while Cassandra is high performance distributed database system.
* MongoDB is written in C++ while Cassandra is written in Java.
* MongoDB is easy to administer in the case of failure while Cassandra provides high availability with no single point of failure.

For more information: [click here](https://www.javatpoint.com/cassandra-vs-mongodb)

---

### 48) Is there any need to create database command in MongoDB?

You don't need to create a database manually in MongoDB because it creates automaically when you save the value into the defined collection at first time.
