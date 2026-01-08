
## 🔗 Architectural Pattern
**Retrieval-Augmented Generation (RAG)** with strict document grounding

---

## 🧩 Component Breakdown

### 📂 Amazon S3 — Source Layer
- Stores all product and client documents
- Organized using prefixes:
  - `product_docs/`
  - `client_docs/`

---

### 🧠 Amazon Bedrock — Intelligence Layer
- Manages:
  - Document ingestion
  - Chunking
  - Embedding generation
  - Retrieval orchestration
- Embedding Model: **amazon-titan-embed-text-v2**

---

### 🔍 OpenSearch Serverless — Vector Store
- Stores embeddings
- Performs semantic similarity search
- Fully managed, no cluster operations

---

### 💬 Amazon Lex — Conversation Layer
- Handles:
  - Intent recognition
  - Utterance routing
  - Structured dialogue
- Delegates retrieval & generation to Bedrock

---

## 🔁 Runtime Flow

1️⃣ User asks a question in Lex  
2️⃣ Intent detected  
3️⃣ Query sent to Bedrock  
4️⃣ Relevant chunks retrieved from OpenSearch  
5️⃣ LLM generates response using retrieved context only  
6️⃣ Answer returned with grounded reasoning  

---

## ✅ Why This Architecture Works for Finance

✔ Prevents hallucinations  
✔ Enforces compliance boundaries  
✔ Supports explainability  
✔ Scales without infra overhead  
