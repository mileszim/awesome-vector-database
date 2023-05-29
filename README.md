# awesome-vector-database

A curated list of awesome vector databases for storing, managing, and searching high-dimensional data. This list includes open-source and commercial solutions, as well as databases that support different types of data and machine learning models.

## Table of Contents

- [Introduction](#introduction)
- [Open Source Databases](#open-source-databases)
    - [Faiss](#faiss)
    - [Annoy](#annoy)
    - [Milvus](#milvus)
    - [HNSWLIB](#hnswlib)
    - [NMSLIB](#nmslib)
- [Commercial Databases](#commercial-databases)
    - [Pinecone](#pinecone)
    - [Vespa](#vespa)
    - [Vector.ai](#vectorai)
    - [Qdrant](#qdrant)
    - [Weaviate](#weaviate)
    - [NucliaDB]
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

6. **[NucliaDB](https://github.com/nuclia/nucliadb)**
    - Description: NucliaDB is a versatile vector database designed for data scientists and machine learning experts working with HuggingFace and other data pipeline platforms. Built on top of the Tantivy library and written in Rust and Python, it is designed to efficiently index large datasets and provide multi-tenant support.
    - Features:
        - Compare vectors from different models
        - Store text, files, vectors, labels, and annotations
        - Annotation and semantic search capabilities
        - Integration with popular NLP pipelines (HuggingFace, PyTorch, etc)
        - Indexing and storage of fields, paragraphs, and semantic sentences
        - Support for multiple fields and metadata, including text, HTML, Markdown, and more
        - Distributed storage layer support with TiKV and Redis
        - PostgreSQL storage layer support for standalone installs
        - Blob support with S3-compatible API, GCS, and PG drivers
        - Replication of index storage and distributed search
    - Pricing and usage: Check out NucliaDB's website for pricing details and usage information, as well as resources like the Quickstart guide, Nuclia Docs, and Developer docs.

## Vector Database Features

When evaluating vector databases, it is essential to consider several key features that can affect performance, usability, and suitability for specific use cases. Here are some of the most important features to consider:

1. **Indexing Methods**: The choice of indexing method can significantly impact the search performance, accuracy, and resource consumption. Common indexing methods include Hierarchical Navigable Small World (HNSW), Inverted File with Product Quantization (IVF-PQ), and Locality-Sensitive Hashing (LSH). Different methods work better for different types of data and use cases, so it is important to select a database that supports the most suitable indexing method for your needs.

2. **Query Types**: Vector databases can support various query types, such as k-nearest neighbors (k-NN), range search, or reverse nearest neighbors (RNN). Some databases also allow combining vector similarity search with other types of queries, such as filtering based on metadata or text search. Consider your specific use case and the types of queries you need to perform when selecting a database.

3. **Scalability and Performance**: The ability to handle large volumes of data and high query loads is a crucial feature for vector databases. Look for databases with distributed architectures, horizontal scalability, and support for data sharding. Additionally, consider the database's performance in terms of query latency, index construction time, and resource consumption, as these factors can impact the overall user experience and the cost of running the system.

4. **Integration with Machine Learning Frameworks**: Many vector database use cases involve working with machine learning models and data processing pipelines. Choose a database that offers seamless integration with popular machine learning frameworks like TensorFlow, PyTorch, or scikit-learn, and supports the data formats and preprocessing steps required for your application.

5. **Data Formats and Storage**: Vector databases can support various data formats, such as dense and sparse vectors, binary data, or text. Some databases also provide support for managing metadata alongside the vector data, allowing for more advanced filtering and querying capabilities. Consider the types of data you need to store and the required storage options, such as on-disk, in-memory, or cloud-based storage.

6. **Security and Privacy**: Data security and privacy are crucial considerations when working with sensitive information. Ensure that the vector database you choose offers features like data encryption, access control, and compliance with relevant regulations (e.g., GDPR, HIPAA). Additionally, consider the database's support for data backup and recovery, as well as options for isolating and managing different data versions.

## Use Cases and Applications

Vector databases are essential in various applications that involve working with high-dimensional data, particularly in machine learning, AI, and analytics. Some common use cases and applications include:

1. **Recommendation Systems**: Vector databases enable efficient similarity search for recommendation systems, allowing for personalized content, product, or service suggestions based on user preferences or item characteristics.

2. **Image and Video Retrieval**: By converting images or video frames into high-dimensional vectors using deep learning models, vector databases can facilitate efficient search and retrieval of visually similar content, such as in image search engines or content-based recommendation systems.

3. **Natural Language Processing (NLP)**: Vector databases are widely used in NLP tasks, such as semantic search, document clustering, or sentiment analysis, where text data is represented as high-dimensional vectors using techniques like word embeddings or sentence embeddings.

4. **Anomaly Detection**: In machine learning applications, high-dimensional data can be used to identify anomalies or outliers in datasets. Vector databases can efficiently search for similar data points and help identify unusual patterns that may indicate fraudulent activity, network intrusions, or equipment failures.

5. **Molecular and Drug Discovery**: In life sciences and pharmaceutical research, vector databases can be used to search and analyze large collections of molecular structures or drug candidates, enabling researchers to identify potential therapeutic targets or drug candidates with similar properties.

## Related Resources

1. **Machine Learning Frameworks**: Popular machine learning frameworks like TensorFlow, PyTorch, or scikit-learn are often used in conjunction with vector databases for data preprocessing, feature extraction, and model training. These frameworks can be integrated with vector databases to enable seamless end-to-end machine learning pipelines.
  * [fill out](here)

2. **Vector Embedding Libraries**: Libraries like Gensim, FastText, or spaCy provide tools for generating high-dimensional vector representations of various data types, such as text, images, or graphs. These embeddings can be stored and searched efficiently using vector databases.
  * [fill out](here)

3. **Data Processing and Visualization Tools**: Tools like Pandas, Dask, or Apache Arrow can be used to preprocess and manipulate large datasets before storing them in vector databases. Visualization tools like Matplotlib, Seaborn, or Plotly can help analyze and visualize high-dimensional data and query results.
  * [fill out](here)

4. **Distributed Computing Frameworks**: In some cases, vector databases can be integrated with distributed computing frameworks like Apache Spark, Hadoop, or Dask to enable large-scale data processing and analytics across multiple nodes or clusters.
  * [fill out](here)

5. **Data Storage and Infrastructure**: Cloud-based storage solutions like Amazon S3, Google Cloud Storage, or Microsoft Azure Blob Storage can be used in conjunction with vector databases to store large volumes of data. Additionally, containerization and orchestration tools like Docker and Kubernetes can help deploy and manage vector databases in various environments, including on-premises, cloud, or hybrid deployments.
  * [fill out](here)
- Research Papers and Articles
- Benchmarking and Evaluation
- Community and Support
