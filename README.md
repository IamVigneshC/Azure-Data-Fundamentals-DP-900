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

A key-value store is the simplest (and often quickest) type of NoSQL database for inserting and querying data. Each data item in a key-value store has two elements, a key and a value. The key uniquely identifies the item, and the value holds the data for the item.




