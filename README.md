# AWS GenAI Financial Advisory Chatbot (RAG-based)

This project implements a domain-specific financial advisory chatbot using
Amazon Lex, Amazon Bedrock, and OpenSearch Serverless.

The chatbot provides **grounded, compliant, and explainable responses**
for DTC financial clients by leveraging Retrieval-Augmented Generation (RAG)
over internal product and client documentation.

The goal of this project is to gain **hands-on experience across the GenAI
project lifecycle**:
- Data ingestion and preparation
- Knowledge base creation using embeddings
- Vector search with OpenSearch
- Conversational interface using Amazon Lex
- Foundations for MLOps and scalable deployment

### 🧠 Solution Overview
Financial advisory workflows require accurate, explainable, and compliant
recommendations grounded in internal documents such as product brochures,
risk disclosures, and client eligibility constraints.

Traditional chatbots hallucinate responses and fail to respect regulatory
or contractual boundaries.

This project addresses those limitations using a RAG-based architecture
that ensures all responses are grounded in approved source documents.

### 🧠 Solution Overview
We implemented a Retrieval-Augmented Generation (RAG) architecture using
AWS-native GenAI services:

- Amazon S3 for document storage
- Amazon Bedrock Knowledge Bases for embeddings and retrieval
- Amazon Titan Embeddings v2 for vectorization
- Amazon OpenSearch Serverless as the vector database
- Amazon Lex for intent-driven conversational interactions

### 🚀 Key Capabilities
- Product recommendations based on client risk appetite and ROI expectations
- Compliance validation using client legal and regulatory constraints
- Risk explanation and eligibility checks
- Grounded answers retrieved directly from source documents


