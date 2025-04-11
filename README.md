# GraphRAG-with-Llama-3.1

GraphRAG-with-Llama-3.1 is an end-to-end demonstration of a retrieval-augmented generation (RAG) pipeline that integrates a graph database (Neo4j) with OpenAI’s Llama models via the **llama-index** library. By leveraging graph structures to represent entities and relationships extracted from unstructured text, this project highlights how embedding semantic context within a graph enhances both retrieval precision and the quality of generative answers.

## Key Features

- **Graph-based Ingestion**: Parse raw text into nodes and relationships in Neo4j using Py2Neo and APOC procedures. Model complex entity relationships (e.g., people, organizations, events) instead of flat document shards.
- **Graph-Driven Indexing**: Extract subgraphs or context windows around query-relevant nodes and build llama-index–friendly indices, enabling targeted retrieval rather than brute-force similarity search over entire documents.
- **RAG Workflows**: Combine graph traversal results with Llama’s generative capabilities to answer questions that require both structured context (from Neo4j) and unstructured synthesis (from the Llama model).
- **Modular Notebook**: A Jupyter notebook (`enhancing_rag_with_graph.ipynb`) walks you through each step—from environment setup and data ingestion to index construction and query execution—so you can adapt the pipeline to your own data.

