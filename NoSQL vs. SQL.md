[[SQL]] databases are [[Relational database|relational]], and [[NoSQL]] are non-relational.

SQL databases use structured query language (SQL) and have a predefined [[Schema|schema]]. NoSQL databases have dynamic schemas for unstructured data.

SQL is vertically scalable, while NoSQL is horizontally scalable. SQL databases are table-based, while NoSQL databases are document, key-value, graph or wide-column stores. SQL is better for multi-row transactions while NoSQL is better for unstructured data like documents or JSON.

NoSQL is preferred over SQL in many cases because it offers more flexibility and scalability. the primary benefit of using a NoSQL system is that it provides developers with the ability to store and access data quickly and easily, without the overhead of a traditional relational database. development teams can focus on delivering features and core business logic faster, without worrying about the underlying data storage implementation. 

the decision of which type of database to use will depend on the particular needs and requirements of the project. 

if you need a fast, scalable, and reliable database for web applications then a NoSQL system may be preferable; if your application requires complex data queries and transactional support then an SQL system is the better choice. 

| Category    | SQL                                                         | NoSQL                                                          |
| ----------- | ----------------------------------------------------------- | -------------------------------------------------------------- |
| type        | [[Relational database\|relational]]                         | non-relational                                                 |
| structure   | uses [[SQL]] + predefined [[Schema\|schema]]                | dynamic schemas for unstructured and semistructured data       |
| scalability | vertically                                                  | horizontally                                                   |
| stores      | table-based                                                 | document, [[Key-Value Pair\|key-value]], graph, or wide-column |
| used for    | multi-row transactions                                      | unstructured data like documents, or [[JSON]]                  |
|             | data is stored in tables with columns and rows              | stored in collections or documents                             |
| examples    | MySQL, PostgreSQL, Oracle, SQL Server, Microsoft SQL Server | MongoDB, Cassandra, Couchbase, Amazon DynamoDB, Redis          |
