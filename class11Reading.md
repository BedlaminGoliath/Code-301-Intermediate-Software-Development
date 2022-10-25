# Class 11 reading

## What kind of data is a good fit for an SQL database? Give a real world example

This comes in the form of Table data bases, which I would be along the lines of a business daily and hourly sales. This way We are able to see the data broken down column by column. This way the Data base is primarly predefined.

## What kind of data is a good fit a NoSQL database? Give a real world example

a NoSQL DB is good for dynamic info from which you are collecting data (like a pie chart/or graph) Here we are able to adjust, the height of whatever N object corrisponds with. I would tie this example to where we collect data (like numer of clicks per item... odd duck) and then relay that graph into a chart.

## Which type of database is best for hierarchical data storage?

NoSQL is better for this type of storage, because it follows the "key-value pair" (much like a JSON file).

NoSQL is prefered for large data.

## Which type of database is best for scalability?

SQL. You can compensate the increased load y increasing CPU,RAM, and SSD.on a single server.

However you can do the same with NoSQL by adding more servers.

SQL are great for heavy transactional based apps and is more stable so I would say that SQL is best for scalabilty.

## SQL vs NoSQL

## What does SQL stand for?

Structered Query Language

Its a language that allows you to write DB querys. This comes with diferent keywords that allows us to select certain fields, we can even insert, remove, or update our data query.

`` SELECT is,name,price FROM products
``

Fields (columns), Records(rows)

## What is a relational database?

table is like a data-bin (storage container). Within  SQL database we have a distinct schema. We also need to have key value pairs (i think). All records within a certain schema need to adhire to that specfic layout.

This is a collection of tables that are tied to one another that relate to one another. Be each table need to be normalized you cannot have empty columns with no info so we create another table that will corrilate with one another.

## What type of structure does a relational database work with?

Many-to-many / one-to-one / one-to-many

## What is a ‘schema’?

The layout or a layout scheme.

## What is a NoSQL database? How does it work?

MongoDB (hummungus it can store lots of data) is a NoSQL database. This looks like a tree where at the top we would have our database, we then go down to our "collections"  (this can be your specific user account and previous orders) we then go down from there we would go down to "documents" which would branch out to said "users" or even multiple "products". This looks like JSON, the other great thing is that is does not have to use the same schema and there is no implied schema. Therefore we could leave empty spaces.

There are no relations. in an NoSQL world, but you have to merge them manually.


## What is inside of a Mongo database?

In mongoDb we have collections. And That way we are able to do collections with no specific schema.

## Which is more flexible - SQL or MongoDB? and why

This seems to be based on what type of app you are building. I Think i agree with the guy in the video where he says you can you use both. For various reasons, In some instances it seems to make sense to make use of the relations. However from my understanding I like the way NoSQL seems to be alittle more flexible within the context of my current uses... horizontal scaling seems to be the deal breaker, due to the scaling

## What is the disadvantage of a NoSQL database?

The disadvantage would be the lack of a schema which would make for to update several different collections instead of having them all in one area. There are instances where we need to update user input. The other downside would be the lack of a schema would make it hard to see if everything is where you need it, because the lack of the schema.


## over all notes

SQL is also called Relational Databases (RDBMS) Or distributed databases.

SQL are table bases, whil NoSQL are doc. based, Key Value pairs, graph databases or wide-column stores.

SQL are vertically scalable, NoSQL or horizontal. SQL are scaled by increasomg horse-power in hardware while NoSWL us DB servers.

SQL uses structure query lanquage.
NoSQL are focused on Doc. based.

UnQL = unstructured query.

complex = SQL (cause its structured)
not complex = NoSQL.

SQL has better cust. service, while NoSQL is more community support.

SQL emphasis on ACID ( Atomicity Consistency Isolation and Durability.)
NoSql emphasis is on Brewers Cap. (Consistency, Availibilty and Partition Tolerance).

Highlevel SQL databases are clssified as Open-sourced or closed-sourced from comm. vendors. NoSQLDB are classified on the basis of way of storing data as graph based DB, Key-value store DB..

### CRUD

four basic operations (create, read, update, and delete) of data storage.

### MongoDB

Mongo is a database (it is storage).

kind of like local storage or cache objects (but better).

### Atlas

This is a cloud platform that will sere mongo DB


cloud?
