# cosmoDB-lab

- 1.Cosmo DB Concepts
    - 1.1 Horizotal Scaling
    - 1.2 Non-Relational

## 1. Cosmo DB Concepts

### 1.1 Horizotal Scaling

In Cosmos DB, horizontal scaling is achieved through the concept of partitions. A partition is a unit of distribution and scalability in Cosmos DB, and it represents a subset of your data stored in a collection. By partitioning your data, you can distribute it across multiple physical partitions, allowing for parallel processing and improved performance.

![alt](/assets/img/horizontally-sclalable.jpg)

CPU and storage resources across physical partitions is dynamically managed by the Cosmos DB service based on the workload and throughput requirements of your application. 

Resume: Each physical partition is assigned its own CPU and storage resources, and the management of these resources is handled by the Cosmos DB service.

### 1.2 Non-Relational

In Cosmos DB, data is stored in documents, which are self-contained JSON objects. 

![alt](/assets/img/relational-workloads.jpg)

Cosmos DB is a NoSQL database that provides a schema-less data model, allowing flexibility in the structure of the documents. Unlike traditional relational databases, Cosmos DB does not enforce referential integrity or provide built-in support for joins between documents.



Step 1 - transform your schemas in json, use camel case in json world and each document need to have the "id" attribute.

![alt](/assets/img/relational-workloads_webstore.jpg)
![alt](/assets/img/relational-workloads_webstore_noSQL.jpg)
![alt](/assets/img/relational-workloads_webstore_noSQL_wrong.jpg)
![alt](/assets/img/relational-workloads_webstore_noSQL_converting.jpg)
![alt](/assets/img/relational-workloads_webstore_noSQL_converting_better.jpg)
![alt](/assets/img/relational-workloads_webstore_noSQL_converting_better_embed.jpg)
![alt](/assets/img/relational-workloads_webstore_noSQL_converting_better_embed_reference.jpg)



## References

()[https://www.youtube.com/watch?v=gqULZ4GIRuY]