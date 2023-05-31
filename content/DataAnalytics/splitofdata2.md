# Split of Data (Cont)

[prev](./splitofdata1.md.md) | [home](./introduction.md)  | [next]()

## Analytical Data

As more businesses move to digital processes, they increasingly recognize the value of being able to respond to opportunities by making faster and well-informed decisions. The above models present the following challenges:

* Ability to run advanced analytics on near-real-time data (streaming data,,social media data, IOT data, etc)
* Need to cleanse the data before using it for aggregation

With the boom of Big Data (Data arriving in varied Variety with high Velocity in large volumes) there was a transition from Extracting, Transforming and Loading data (ETL) to **Extracting,Loading and then Transforming data(ELT)** for meaningful insights. This was primarily to address 3 V's Variety,Velocity & Volume. Following patterns evolved which focussed on prioritizing storage volume and cost over performance.

### 5) Data Lakes

A data lake captures anything the organization deems valuable for future use.Essentially  it serves as a central repository that holds a large amount of data in its native, raw format. This approach differs from a traditional data warehouse, which transforms and processes the data at the time of ingestion.Its optimized to for scaling from gigabytes to terabytes and petabytes of data. They are built to handle high volumes of small writes at low latency, and are optimized for massive throughput.

Typically this transformation uses an **ELT (extract-load-transform)** pipeline, where the data is ingested and transformed in place. Source data that is already relational may go directly into the data warehouse, using an ETL process, skipping the data lake.

A following table will help to make your use case clearer
![Comparison Table](/images/ComparisonLakevsWarehouse.png)

#### When to use Data Lake solutions

* Data lake stores are often used in event streaming or IoT scenarios, because they can persist large amounts of relational and nonrelational data without transformation or schema definition.

### 6) Delta Lakes

Delta Lake is an open-source storage layer that brings ACID (atomicity, consistency, isolation, and durability) transactions to Apache Spark and big data workloads.

## Additional Information

* [Big Data Characteristics](https://www.teradata.com/Glossary/What-are-the-5-V-s-of-Big-Data#:~:text=Big%20data%20is%20a%20collection,variety%2C%20velocity%2C%20and%20veracity) 
* [Data Lakes](https://learn.microsoft.com/azure/architecture/data-guide/scenarios/data-lake)