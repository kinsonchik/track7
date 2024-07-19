# Adding Hardware spec details
Last Updated: 2024-07-03
Milvus is a vector database that stores, indexes, and manages massive embedding vectors that are developed by deep neural networks and other machine learning (ML) models. It is developed to empower embedding similarity search and AI applications. Milvus makes unstructured data search more accessible and consistent across various environments.

## Details
| Software | vCPU | Memory | Storage | Notes |
| ----- | ----- | ----- | ---- | ----- |
| watsonx.data	| Operator pods: \n 1 vCPU \n Catalog pods: 0.01 vCPU \n Operand: 20 vCPU | Operator pods: \n 0.75 GB RAM \n Catalog pods: 0.05 GB RAM \n Operand: 62 GB RAM Persistent storage: 542 GB \n Ephemeral storage:  25 GB \n Image storage: Up to 19.91 GB | Minimum resources for an installation with a single replica of the Presto engine. | If you increase the number of Presto replicas, you need additional vCPU, memory, and ephemeral storage. Work with IBM Sales to get a more accurate sizing based on your expected workload. If Analytics Engine powered by Apache Spark is not installed, add the vCPU and memory required for Analytics Engine powered by Apache Spark to the information listed for watsonx.data.

Content curated from:
- [https://cloud.ibm.com/docs/watsonxdata?topic=watsonxdata-adding-milvus-service](https://www.ibm.com/docs/en/cloud-paks/cp-data/5.0.x?topic=requirements-hardware)
