# Azure-Data-Fundamentals-DP-900


- Descriptive analytics examines what happened in the past (What's happening?)
- Diagnostics analytics identifies trends or patterns in the past and then goes a step further to explain why the trends occurred the way they did (Why happening?)
- Predictive analytics is what it sounds like — it aims to predict likely outcomes and make educated forecasts using historical data (What will happen?)
- Prescriptive analytics uses the data from a variety of sources — including statistics, machine learning, and data mining — to identify possible future outcomes and show the best option (What actions should we take?)

------------------------------------------------

- Normalization is the process of **organizing data** in a database. This includes creating tables and **establishing relationships** between those tables according to rules designed both to protect the data and to make the database more flexible by **eliminating redundancy and inconsistent dependency**.

------------------------------------------------

- Extratct Load Transform (ELT) requires a target data store powerful enough to transform data
- Extratct Transform Load (ETL) requires data that is fully processed before being loaded to the target data store

-----------------------------------------------
Star Schema in data warehouse, in which the center of the star can have one fact table and a number of associated dimension tables. It is known as star schema as its structure resembles a star.Dimension tables describe business entities—the things you model. Entities can include products, people, places, and concepts including time itself.Fact tables store observations or events, and can be sales orders, stock balances, exchange rates, temperatures, etc. A fact table contains dimension key columns that relate to dimension tables, and numeric measure columns.

https://docs.microsoft.com/en-us/power-bi/guidance/star-schema
https://learn.microsoft.com/en-us/training/modules/explore-fundamentals-data-visualization/3-data-modeling

------------------------------------------------
MPP distributes processing across compute nodes

https://learn.microsoft.com/en-us/azure/synapse-analytics/sql-data-warehouse/massively-parallel-processing-mpp-architecture


