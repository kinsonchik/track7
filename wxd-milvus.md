# Adding Milvus service
Last Updated: 2024-07-03
Milvus is a vector database that stores, indexes, and manages massive embedding vectors that are developed by deep neural networks and other machine learning (ML) models. It is developed to empower embedding similarity search and AI applications. Milvus makes unstructured data search more accessible and consistent across various environments.

## Procedure
- Complete the following steps to add Milvus as a service in IBM® watsonx.data.
  - Log in to the watsonx.data console.
  - From the navigation menu, select Infrastructure Manager.
  - To define and connect to a service, click Add component and select Add service.
  - In the Add service window, select Milvus from the Type list.
    
| Field | Description |
| ----- | ---------- |
|Display name|	Enter the Milvus service name to be displayed on the screen.|
|Size	|Select the suitable size.|
||Starter: Recommended for 1 million vectors, 64 index parameters, 1024 segment size, and 384 dimensions.|
||Small: Recommended for 10 million vectors, 64 index parameters, 1024 segment size, and 384 dimensions.|
||Medium: Recommended for 50 million vectors, 64 index parameters, 1024 segment size, and 384 dimensions.|
||Large: Recommended for 100 million vectors, 64 index parameters, 1024 segment size, and 384 dimensions.|
|Add storage bucket|	Associate an external bucket for the Small, Medium, or Large sizes. For Starter size, you can also select an IBM-managed bucket. To associate an external bucket, you must have the bucket configured.|
|Path|	For external buckets, specify the path where you want to store vectorized data files.|

Content curated from:
- https://cloud.ibm.com/docs/watsonxdata?topic=watsonxdata-adding-milvus-service
