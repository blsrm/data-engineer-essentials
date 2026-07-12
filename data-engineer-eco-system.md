# Core Big Data Concepts
## Big Data
Large amounts of data that cannot be processed on one computer. Needs distributed systems.

## Hadoop
An open‑source framework to store and process big data across many machines.

## HDFS (Hadoop Distributed File System)
Storage layer of Hadoop.
Stores huge files by splitting them into blocks and distributing across machines.

MapReduce
Processing layer of Hadoop.
Breaks a job into:

Map → split work

Reduce → combine results

Cloudera
A company that provides enterprise Hadoop distributions and tools.

2. SQL & Warehousing
SQL
Language to query and manipulate data in databases.

Warehouse / SQL Warehouse
A system optimized for analytics (not transactions).
Stores structured data and runs fast SQL queries.

ACID
Database properties:

Atomic

Consistent

Isolated

Durable
Ensures reliable transactions.

CDC (Change Data Capture)
Technique to capture only changed data (inserts/updates/deletes).

Incremental Loads
Loading only new or changed data instead of full data every time.

