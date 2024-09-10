# Redis Interview Questions

A list of frequently asked **Redis interview questions** and answers are given below.

---

### 1) What is Redis?

Redis is an open-source, advance key value data store and cache. It is also referred as a data structure server which keys not only contains strings, but also hashes, sets, lists, and sorted sets.

---

### 2) What is the meaning of Redis?

Redis stands for REmote DIctionary Server.

---

### 3) How is Redis different from other databases?

Redis is a NoSQL, Opensource, in-memory data-structure store. It follows the principle of key-value store.

It is extremely fast, persistent, portable and supports many languages such as C, C++, C#, Clojure, Common Lisp, D, Dart, Erlang, Go, Haskell, Haxe, Io, Java, JavaScript (Node.js), Julia, Lua, Objective-C, Perl, PHP, Pure Data, Python, R, Racket, Ruby, Rust, Scala, Smalltalk and Tcl.

**For more information:[Click Here](https://www.javatpoint.com/redis-vs-other-key-value-stores)**

---

### 4) In which language Redis is written?

Redis is written in ANSI C and mostly used for cache solution and session management. It creates unique keys for store values.

---

### 5) What is the usage of Redis?

Redis is a special key-value store database that can function as a NoSQL database or as a memory-cache store to improve performance when serving data that is stored in system memory.

---

### 6) How to interect with Redis?

After the installation of the server you can run the Redis Client provided by redis installation or you can open the command prompt and use the following command:

By using any of them, you can interect with Redis.

---

### 7) Which are the most popular companies using Redis?

Twitter, Github, Stackoverflow etc. are the most popular companies using Redis.

---

### 8) What are the main features of Redis?

Following are the main features of Redis:

* Redis is very simple to install setup and manage.
* Redis is very fast. It can execute 100000 queries per second.
* Redis is fast because data is being persistent in memory as well as stored on the disk.
* Redis is very fast because it loads the whole dataset in primary memory.
* Redis operations working on different data types are atomic so these operations can be accomplished safely i.e. to set or increase a key, add or remove elements from a set or increase a counter.
* It supports various types of data structure such as strings, hashes, sets, lists, sorted sets etc.
* Redis supports a variety of languages i.e. C, C++, C#, Ruby, Python, Twisted Python, PHP, Erlang, Tcl, Perl, Lua, Java, Scala etc. 
* If your favorite language is not supported yet, you can write your own client library, as the Protocol is pretty simple.
* Redis supports simple master to slave replication.
* Redis is portable.

**For more information:[Click Here](https://www.javatpoint.com/features-of-redis)**

---

### 9) Explain the Replication Features of Redis? 

Replication is important in order to archive high level of availability in big data systems. The data needs to be replicated at n number of places. This follows the master-slave approach where the master copy is maintained by master-slave and replicated to n other nodes. 

---

### 10) What are the advantages of using Redis?

Following is a list of some important advantages of Redis:

* Redis is very fast.
* It supports a server-side locking.
* It has a rich client side library.
* It is a good counter.
* It supports Atomic Operation.

---

### 11) What are the disadvantages/limitations of using Redis?

Following are the disadvantages/ limitations of Redis:

* It is single threaded.
* It has got limited client support for consistent hashing.
* It has significant overhead for persistence.
* It is not deployed widely.

---

### 12) What is the difference between Redis and RDBMS?

There are a lot of differences between Redis and RDBMS:

* Redis is a NoSQL database while RDBMS is an SQL database.
* Redis follows the key-value structure while RDBMS follows the table structure.
* Redis extremely fast while RDBMS is comparatively slow.
* Redis stores all the dataset in primary memory while RDBMS stores its dataset in secondary memory.
* Redis is generally used to store small and frequently used files while RDBMS is used to store big files.
* Redis provides only official support for Linux, BSD, Mac OS X, Solaris. It doesn?t provide official support for Windows currently while RDBMS provides support for both.

**For more information:[Click Here](https://www.javatpoint.com/redis-vs-rdbms)**

---

### 13) Differentiate Memcached and Redis? 

| Memcached                                                                                                                | Redis                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------- |
| Memcached only does caching information.                                                                                 | It provides some more functionalities like replication and persistence along with caching information.                              |
| Memcached supports the functionality of LRU (Least Recently Used) eviction of values.                                    | LRU is not supported by Redis.                                                                                                      |
| In Memcached, when they overflow memory, the one you have not used recently (LRU- Least Recently Used) will get deleted. | In Redis, there is a time set for each function, Three keys are maintained, the one, which is closest to expiry, will get deleted.  |
| CAS (Check and Set) is supported by Memcached.                                                                           | CAS is not supported by Redis.                                                                                                      |
| Array objects are needed to be serialized in order to get saved. We need to unserialize them for their retrieval.        | Redis has got stronger data structures; it can handle strings, binary safe strings, list of binary safe strings, sorted lists, etc. |
| Memcached has at most 250 bytes length.                                                                                  | Redis has at most 2 GB key length.                                                                                                  |
| It is Multi-threaded                                                                                                     | It is single threaded.                                                                                                              |

---

### 14) Mention Operation Keys of Redis. 

* TYPE key
* TTL key
* EXPIRE key seconds
* EXPIREAT key timestamp
* EXISTS key
* DEL key

---

### 15) Which are the different data types used in Redis?

There are mainly 5 types of data types supported by Redis:

* Strings
* Hashes
* Lists
* Sets
* Sorted Sets

**For more information:[Click Here](https://www.javatpoint.com/redis-data-types)**

---

### 16) Which are the most popular commands of the Redis database?

**For more information:[Click Here](https://www.javatpoint.com/redis-all-commands)**

---

### 17) We all know that Reds is fast, but is it also durable?

In Redis, there is always a trade-of between durability and speed. In the case of system failure, it may lose data which is not stored.

---

### 18) How can you enhance the durability of Redis? 

* Whenever a new command is added to the append log file, call Fsysnc() each time. 
* Keep calling Fsysnc() in every second. Despite of the 1 second data lose in the case of system fails. 

---

### 19) What are the concerned things while using Redis? 

* Consistent method selection in order to name and prefix the keys. Namespace management. 
* Make key prefixes registry which can map every documents to their owner applications. 
* Designing, implementing and testing the Garbage collection mechanism for each class we keep into the redis architecture. 
* Maintain a sharding library before investing so much into the application. 

---

### 20) How can you use Redis with .Net application?

To use Redis in .Net applications, follow these steps:

* First, Download Redis Server.
* Install Redis Server.
* Download Redis Client.
* Set Configuration into Web.config File.
* Use Redis Client Class.
