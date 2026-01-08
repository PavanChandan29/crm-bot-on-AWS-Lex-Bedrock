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

### Problem Statement
Financial advisory workflows require accurate, explainable, and compliant
recommendations grounded in internal documents such as product brochures,
risk disclosures, and client eligibility constraints.

Traditional chatbots hallucinate responses and fail to respect regulatory
or contractual boundaries.

This project addresses those limitations using a RAG-based architecture
that ensures all responses are grounded in approved source documents.
