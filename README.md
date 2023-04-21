# awesome-vector-database

A curated list of awesome vector databases for storing, managing, and searching high-dimensional data. This list includes open-source and commercial solutions, as well as databases that support different types of data and machine learning models.

## Table of Contents

- [Introduction](#introduction)
- [Open Source Databases](#open-source-databases)
- [Commercial Databases](#commercial-databases)
- [Vector Database Features](#vector-database-features)
- [Use Cases and Applications](#use-cases-and-applications)
- [Related Resources](#related-resources)

## Introduction

Vector databases are essential tools for storing, managing, and searching large volumes of high-dimensional data. They are widely used in machine learning, artificial intelligence, and other data-intensive applications. This list provides an overview of the most popular and powerful vector databases, along with a summary of their key features and use cases.

## Open Source Databases

1. **[Faiss](https://github.com/facebookresearch/faiss)**
    - Description: Faiss is a library developed by Facebook AI Research that provides efficient similarity search and clustering of dense vectors. It is designed for use with large-scale, high-dimensional data and supports several index types and algorithms for various use cases.
    - Features:
        - GPU and CPU support
        - Indexing methods: LSH, PQ, HNSW, and more
        - Clustering algorithms: k-means, PCA
        - Python and C++ interfaces
    - Installation and usage: Faiss can be installed using pip or conda, and its API is well-documented with examples available in the official repository.

2. **[Annoy](https://github.com/spotify/annoy)**
    - Description: Annoy (Approximate Nearest Neighbors Oh Yeah) is a C++ library created by Spotify for approximate nearest neighbor search. It is memory-efficient and optimized for fast query times. Annoy is particularly useful when dealing with large datasets, and it supports static and dynamic datasets.
    - Features:
        - Static and dynamic index support
        - Memory-mapped files for sharing indices between processes
        - Custom distance metrics: Euclidean, Manhattan, Angular, and more
        - Python, C++, and other language bindings
    - Installation and usage: Annoy can be installed using pip, and it has an easy-to-use Python API with examples and tutorials available on the project's GitHub page.

3. **[Milvus](https://github.com/milvus-io/milvus)**
    - Description: Milvus is an open-source vector database built for AI and analytics applications. It supports multiple index types and provides powerful scalability and performance. Milvus is designed for managing massive high-dimensional data and enables efficient similarity search and analytics.
    - Features:
        - GPU and CPU support
        - Indexing methods: IVF, HNSW, PQ, and more
        - Hybrid search: combining scalar and vector filtering
        - RESTful API and Python, Java, Node.js, and C++ SDKs
        - Horizontal scalability and data sharding
    - Installation and usage: Milvus can be installed using Docker or built from source, and it comes with extensive documentation and examples to help you get started.

4. **[HNSWLIB](https://github.com/nmslib/hnswlib)**
    - Description: HNSWLIB is an open-source C++ library for approximate nearest neighbor search, which implements the Hierarchical Navigable Small World (HNSW) algorithm. It is designed for high-performance similarity search in large-scale datasets with various distance metrics.
    - Features:
        - Fast query performance
        - Support for multi-core parallelism
        - Custom distance metrics: Euclidean, Cosine, L1, and more
        - Python and C++ interfaces
    - Installation and usage: HNSWLIB can be installed using pip, and its API is easy to use with Python and C++ examples provided in the official repository.

5. **[NMSLIB](https://github.com/nmslib/nmslib)**
    - Description: Non-Metric Space Library (NMSLIB) is an open-source, highly efficient library for similarity search and nearest neighbor search in generic metric and non-metric spaces. It supports various similarity search algorithms and distance functions, making it suitable for a wide range of applications.
    - Features:
        - Indexing methods: HNSW, SW-graph, VPTree, and more
        - Custom distance metrics: Euclidean, Cosine, Jaccard, and more
        - Efficient index construction and query processing
        - Python, C++, and Java bindings
    - Installation and usage: NMSLIB can be installed using pip or built from source, and it offers a Python API with examples and documentation available on the project's GitHub page.

## Commercial Databases

1. **[Pinecone](https://www.pinecone.io)**
    - Description: Pinecone is a managed vector database designed for large-scale machine learning applications. It provides a simple API for creating and managing vector indices, enabling fast and accurate similarity search across billions of items.
    - Features:
        - Managed service with autoscaling
        - Indexing methods: HNSW, PQ, and more
        - Python, Java, and RESTful API
        - Data versioning and rollback
        - Integration with popular machine learning frameworks
    - Pricing and usage: Pinecone offers a free tier with limited resources, as well as pay-as-you-go and enterprise plans with additional features and support.

2. **[Vespa](https://vespa.ai)**
    - Description: Vespa is a real-time, scalable search, recommendation, and analytics engine developed by Yahoo. It supports efficient similarity search on high-dimensional vectors and allows for complex queries combining structured and unstructured data.
    - Features:
        - Real-time indexing and search
        - Indexing methods: HNSW, ANN, and more
        - Support for structured data and text search
        - RESTful API and Java, Python, and Node.js clients
        - Distributed architecture with horizontal scalability
    - Pricing and usage: Vespa is available as a managed service on the Vespa Cloud platform, with pricing based on resource consumption and data storage. A self-hosted option is also available for on-premises or cloud deployment.

3. **[Vector.ai](https://github.com/vector-ai/vectorai)**
    - Description: Vector.ai is a managed vector search platform that provides an API for creating, managing, and searching vector indices. It is designed to handle large volumes of high-dimensional data, enabling efficient similarity search for machine learning and AI applications.
    - Features:
        - Managed service with autoscaling
        - Indexing methods: HNSW, PQ, and more
        - Python and RESTful API
        - Data versioning and backup
        - Integration with popular machine learning frameworks
    - Pricing and usage: Vector.ai offers a free tier with limited resources, as well as paid plans with additional features, support, and custom pricing for enterprise customers.

4. **[Qdrant](https://github.com/qdrant/qdrant)**
    - Description: Qdrant is a high-performance vector search engine designed for efficient similarity search and management of large-scale, high-dimensional data. It offers a flexible API and a wide range of indexing methods, making it suitable for various use cases.
    - Features:
        - GPU and CPU support
        - Indexing methods: HNSW, IVF, and more
        - RESTful API and Python, Java, Node.js, and C++ SDKs
        - Data filtering and aggregation
        - Horizontal scalability and sharding
    - Pricing and usage: Qdrant offers a free trial with limited resources, as well as paid plans and custom enterprise pricing based on data storage and query volume.

5. **[Weaviate](https://github.com/weaviate/weaviate)**
    - Description: Weaviate is an open-source, GraphQL-based vector search engine that enables similarity search on high-dimensional data. While it is open-source, the commercial version offers additional features, support, and managed services.
    - Features:
        - Support for various data types: text, images, audio, and more
        - Indexing methods: HNSW, ANN, and more
        - GraphQL and RESTful API
        - Real-time search and indexing
        - Integration with machine learning frameworks
    - Pricing and usage: Weaviate offers a free open-source version and a commercial version with additional features and managed services. Pricing for the commercial version depends on the resources needed and is available upon request.

## Vector Database Features

- Indexing Methods
- Query Types
- Scalability and Performance
- Integration with Machine Learning Frameworks
- Data Formats and Storage
- Security and Privacy

## Use Cases and Applications

1. Image and Video Retrieval
2. Natural Language Processing and Information Retrieval
3. Recommender Systems
4. Anomaly Detection
5. Bioinformatics and Genomics
6. Geospatial Data Analysis

## Related Resources

- Tutorials and Guides
- Research Papers and Articles
- Benchmarking and Evaluation
- Community and Support
