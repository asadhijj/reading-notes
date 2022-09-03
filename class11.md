# Mongo and Mongoose 

Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

![Object Mapping between Node and MongoDB managed via Mongoose](./assets/mongoose.png)

MongoDB is a schema-less NoSQL document database. It means you can store JSON documents in it, and the structure of these documents can vary as it is not enforced like SQL databases. This is one of the advantages of using NoSQL as it speeds up application development and reduces the complexity of deployments.

***
## SQL vs NoSQL

1. **Fill in the chart below with five differences between SQL and NoSQL databases:**

|SQL                              |NoSQL                            |
|---------------------------------|---------------------------------|
|table based                      |document based                   |
|predefined shcema                |dynamic schema                   |
|vertically scalable              |horizontally scalable            |
|good for complex quereis         |not good for complex queries     |
|bad for hierarchical data storage|bad for hierarchical data storage|

2. **What kind of data is a good fit for an SQL database? give examples**

    Numeric data types such as int, tinyint, bigint, float, real, etc.
    Date and Time data types such as Date, Time, Datetime, etc.
    Character and String data types such as char, varchar, text, etc.
    Unicode character string data types, for example nchar, nvarchar, ntext, etc.
    Binary data types such as binary, varbinary, etc.
    Miscellaneous data types - clob, blob, xml, cursor, table, etc.

3. **What kind of data is a good fit a NoSQL database?**

   * Key-value Pair 

   * Column-oriented Graph 

   * Graphs based 

   * Document-oriented 


Based  all web applications require user profiles and the ability to log in. A global user profile store is another example of where the key value characteristics of NoSQL come into play

4. **Which type of database is best for hierarchical data storage?**
  SQL > NoSQL


5. **Which type of database is best for scalability?**

  NoSQL > SQL

***

1. **What does SQL stand for?**
Structured Query Language

2. **What is a relational database?**
a type of database that stores and provides access to data points that are related to one anothe

3. **What type of structure does a relational database work with?**
 rows + columns = tables

4. **What is a 'schema'?**
A database schema defines how data is organized within a relational database; this is inclusive of logical constraints such as, table names, fields, data types, and the relationships between these entities

5. **What is a NoSQL database?**
 a database that provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases.

 6. **How does it work?**

 it stores data in 4 different ways 
   *  Key-value Pair 

   * Column-oriented Graph 

   * Graphs based 

   * Document-oriented 

7. **What is inside of a Mongo database?**

records which are made up of documents that contain a data structure composed of keys and value pairs

8. **Which is more flexible - SQL or MongoDB? and why.**

MongoDB is more flexible because it allows to store the data in different ways other than rows and columns.

9. **What is the disadvantage of a NoSQL database?**
 that it doesnt operate with ACID (Atomicity, Consistency, Isolation, and Durability) properties so it doesnt ensure reliability of transactions.

 ***

  ## Things I want to know more about
  i want to learn more about how to interact with databases and how to decide which database is more efficient to use for our applications.

***

## External Sources 

[SQL vs noSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
[SQL vs noSQL video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
[free code camp mongoDB](https://www.freecodecamp.org/news/introduction-to-mongoose-for-mongodb-d2a7aa593c57/)




 



   