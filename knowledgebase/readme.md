# 🧠 Amazon Bedrock Knowledge Base

## 🔧 Configuration Summary

- Embedding Model: **amazon-titan-embed-text-v2**
- Vector Store: **Amazon OpenSearch Serverless**
- Chunking Strategy: **Hierarchical Chunking**

---

## 🧩 Why Hierarchical Chunking?

Financial documents follow natural sections:
- Overview
- Risk
- Returns
- Legal
- Eligibility

Hierarchical chunking:
✔ Preserves semantic boundaries  
✔ Improves retrieval precision  
✔ Reduces context pollution  

---

## 🔄 Synchronization

After vector store creation:
- Knowledge base **must be synced**
- Sync embeds all documents
- Required after:
  - New uploads
  - Document updates

---

## 🎯 Result

✔ Accurate semantic retrieval  
✔ Explainable RAG answers  
✔ Stable vector dimensions  
