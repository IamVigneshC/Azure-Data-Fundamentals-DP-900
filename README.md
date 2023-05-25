# Azure-Data-Fundamentals-DP-900


- Descriptive analytics examines what happened in the past (What's happening?)
- Diagnostics analytics identifies trends or patterns in the past and then goes a step further to explain why the trends occurred the way they did (Why happening?)
- Predictive analytics is what it sounds like — it aims to predict likely outcomes and make educated forecasts using historical data (What will happen?)
- Prescriptive analytics uses the data from a variety of sources — including statistics, machine learning, and data mining — to identify possible future outcomes and show the best option (What actions should we take?)

- https://demand-planning.com/2020/01/20/the-differences-between-descriptive-diagnostic-predictive-cognitive-analytics/ 
- https://azure.microsoft.com/en-us/blog/answering-whats-happening-whys-happening-and-what-will-happen-with-iot-analytics/

------------------------------------------------

- Normalization is the process of **organizing data** in a database. This includes creating tables and **establishing relationships** between those tables according to rules designed both to protect the data and to make the database more flexible by **eliminating redundancy and inconsistent dependency**.

------------------------------------------------

- Extract Load Transform (ELT) requires a target data store powerful enough to transform data
- Extract Transform Load (ETL) requires data that is fully processed before being loaded to the target data store

-----------------------------------------------
Star Schema in data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star.Dimension tables describe business entities—the things you model. Entities can include products, people, places, and concepts including time itself.Fact tables store observations or events, and can be sales orders, stock balances, exchange rates, temperatures, etc. A fact table contains dimension key columns that relate to dimension tables, and numeric measure columns.

- https://docs.microsoft.com/en-us/power-bi/guidance/star-schema
- https://learn.microsoft.com/en-us/training/modules/explore-fundamentals-data-visualization/3-data-modeling

------------------------------------------------
- MPP distributes processing across compute nodes
- https://learn.microsoft.com/en-us/azure/synapse-analytics/sql-data-warehouse/massively-parallel-processing-mpp-architecture

------------------------------------------------
- https://www.w3schools.com/js/js_json_arrays.asp
- https://www.w3schools.com/js/js_json_objects.asp
------------------------------------------------
Clustered indexes sort and store the data rows in the table or view based on their key values. These are the columns included in the index definition. There can be only one clustered index per table, because the data rows themselves can be stored in only one order.

------------------------------------------------

- RDBMS is for the transactional system - OLTP
- https://docs.microsoft.com/en-us/dotnet/architecture/cloud-native/relational-vs-nosql-data
- https://towardsdatascience.com/choosing-the-right-database-c45cd3a28f77


------------------------------------------------
- Treemaps are charts of colored rectangles, with size representing value. They can be hierarchical, with rectangles nested within the main rectangles
- A key influencer chart displays the major contributors to a selected result or value
- Scatter and Bubble charts display relationships between 2 (scatter) or 3 (bubble) quantitative measures -- whether or not, in which order, etc

------------------------------------------------

- A key-value store is the simplest (and often quickest) type of NoSQL database for inserting and querying data. Each data item in a key-value store has two elements, a key and a value. The key uniquely identifies the item, and the value holds the data for the item.
- Azure Table Storage is a NoSQL storage solution that makes use of tables containing key/value data items. Each item is represented by a row that contains columns for the data fields that need to be stored.
- Key-value pairs are a feature of the Table storage of Cosmos DB, Table storage, and Redis cache. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/architecture/data-guide/big-data/non-relational-data

------------------------------------------------
A Data Factory or Synapse Workspace can have one or more pipeline.
- A pipeline is a logical grouping of activities that together perform a task and can be scheduled. The activities in a pipeline define actions to perform on your data.
- A Dataset is a named view of data that simply points or references the data you want to use in your activities as inputs and outputs. Datasets identify data within different data stores, such as tables, files, folders, and documents.

- Before you create a dataset, you must create a linked service to link your data store to the service. Linked services are much like connection strings, which define the connection information needed for the service to connect to external resources. The dataset represents the structure of the data within the linked data stores, and the linked service defines the connection to the data source

------------------------------------------------

There's 3 type of Relational data SQL:

- DDL (Data Definition Language) CREATE, DROP, ALTER, RENAME, COMMENT AND TRUNCATE.
- DML (Data Manipulación Language) SELECT, INSERT INTO, DELETE, UPDATE.
- DCL (Data Control Language) REVOKE & GRANT.
- TCL (Transaccional Control Language) COMMIT & ROLLBACK

------------------------------------------------

Unlimited databases can be created in a single Cosmos DB account. There is no limit to the number of databases in a single Cosmos DB account, currently. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/cosmos-db/concepts-limits

------------------------------------------------

Always Encrypted is a feature designed to protect sensitive data, such as credit card numbers or national identification numbers (for example, U.S. social security numbers), stored in Azure SQL Database or SQL Server databases. Always Encrypted allows clients to encrypt sensitive data inside client applications and never reveal the encryption keys to the Database Engine (SQL Database or SQL Server). As a result, Always Encrypted provides a separation between those who own the data and can view it, and those who manage the data but should have no access. By ensuring on-premises database administrators, cloud database operators, or other high-privileged unauthorized users, can't access the encrypted data, Always Encrypted enables customers to confidently store sensitive data outside of their direct control. This allows organizations to store their data in Azure, and enable delegation of on-premises database administration to third parties, or to reduce security clearance requirements for their own DBA staff. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/sql/relational-databases/security/encryption/always-encrypted-database-engine?view=sql-server-ver15

------------------------------------------------

Zone-redundant storage (ZRS) copies your data synchronously across three Azure availability zones in the primary region. For applications requiring high availability, Microsoft recommends using ZRS in the primary region, and also replicating to a secondary region. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy

------------------------------------------------

Azure SQL Database has a server and database firewall. By default, no IP addresses are allowed to access the database until you add one. Refer to Microsoft Doc: https://docs.microsoft.com/en-us/azure/azure-sql/virtual-machines/windows/ways-to-connect-to-sql


------------------------------------------------

Table Storage is a good solution when you have a large volume of key-value data, and don't want to pay too much to store it. Especially when latency is not a huge issue for you.

------------------------------------------------

Clustered indexes sort and store the data rows in the table or view based on their key values. These are the columns included in the index definition. There can be only one clustered index per table, because the data rows themselves can be stored in only one order. This is also called a PRIMARY KEY.

------------------------------------------------

Object data, which is Azure Blob Storage inside Azure, uses a container metaphor. You can store any type of binary or text data into it, using files. The data store is optimzed for files such as images and videos. 


------------------------------------------------

Redis Cache is charged by the hour, and varies by region. It also depends on the tier you choose. Refer to Microsoft Doc: https://azure.microsoft.com/en-us/pricing/details/cache/



------------------------------------------------

Soft Delete allows you to recover deleted files within a set time period as configured. Change Feed would not allow you to recover deleted files. Immutable blobs can restrict deletion but not help you recover files. And Azure Policy does not have an option that deals with the contents of a storage account.


------------------------------------------------

Transaction Optimized storage provides better a cost profile for frequently accessed files. It costs more to store the file, but much less to access it. And it supports Standard Tier of storage.

------------------------------------------------

The minimum throughput you can allocate to a database or container is 400 RU/s. 

------------------------------------------------

You can configure your storage account to accept requests from secure connections only by setting the Secure transfer required property for the storage account. When you require secure transfer, any requests originating from an insecure connection are rejected. 

------------------------------------------------

The Azure Data Lake uses a driver compatible with the Hadoop File System (HDFS). It is designed to be highly fault-tolerant, provide high throughput access, and is suitable for applications that have large data sets. It runs on top of the underlying disk file system.



------------------------------------------------

Azure Table Storage allows you to store key-value data as the cheapest per GB rate. Cosmos DB also have a key-value option, but is not as cost effective. Azure SQL Database is a relational data store. And Azure Data Lake Storage is a good option for data ingestion, but is not a key-value storage.


------------------------------------------------

SQL injection is an attack in which malicious code is inserted into strings that are later passed to an instance of SQL Server for parsing and execution. Any procedure that constructs SQL statements should be reviewed for injection vulnerabilities because SQL Server will execute all syntactically valid queries that it receives. Even parameterized data can be manipulated by a skilled and determined attacker. 


------------------------------------------------

Resource tokens provide access to the application resources within a database. You can use a resource token (by creating Cosmos DB users and permissions) when you want to provide access to resources in your Cosmos DB account to a client that cannot be trusted with the primary key.

------------------------------------------------

Instead of believing everything behind the corporate firewall is safe, the Zero Trust model assumes breach and verifies each request as though it originated from an uncontrolled network. Regardless of where the request originates or what resource it accesses, the Zero Trust model teaches us to "never trust, always verify.

------------------------------------------------

Transparent Data Encryption (TDE) encrypts SQL Server, Azure SQL Database, and Azure Synapse Analytics data files. This encryption is known as encrypting data at rest. 

------------------------------------------------

- Core (SQL) API stores data in JSON document format
- Table API stores data in key/value format
- Cassandra API stores data in column-oriented schema
- Gremlin API allows users to make graph queries and stores data as edges and vertices
- MongoDB API also uses documents but is BSON format, which is a binary format and not text-based

------------------------------------------------
Azure Databricks has several features, and one includes a complete ML platform where you can build, train and test models.


------------------------------------------------

Cosmos DB Table API offers single-digit millisecond latency for reads and writes, backed with <10 ms latency for reads and writes at the 99th percentile, at any scale, anywhere in the world. It is not less expensive than table storage. They both offer an SLA, and are both programmable. 

------------------------------------------------


Primary keys provide access to all the administrative resources for the database account. Each account consists of two primary keys: a primary key and secondary key. The purpose of dual keys is to let you regenerate, or roll keys, providing continuous access to your account and data.


------------------------------------------------
Data movement, Data transformation, and Control are the three types of activities that Azure Data Factory supports. 

------------------------------------------------
Document data is data that is stored in a readable format, such as JSON. Using Cosmos DB Core SQL API, you can query this data. The database does not enforce a schema on the data. It scales for a global scale.

------------------------------------------------

Azure Databricks offers a SQL platform for analysts to run queries against data, a platform to allow data scientists and engineers to work together on tough data science problems, and a machine learning environment to build, train and test models.

------------------------------------------------


------------------------------------------------
