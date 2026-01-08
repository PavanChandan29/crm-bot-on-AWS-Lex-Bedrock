# 📥 Data Ingestion & Preparation

## 📚 Document Types

### 🧾 Product Documents
- Product description
- Expected returns
- Risk classification
- Legal & regulatory terms
- Eligibility constraints

### 👤 Client Documents
- Risk appetite
- Investment horizon
- ROI expectations
- Legal restrictions
- Suitability conditions

---

## 📂 Storage Strategy

All documents are stored in **Amazon S3** using logical prefixes:

- `product_docs/`
- `client_docs/`

This enables:
✔ Easy lifecycle management  
✔ Clean knowledge base ingestion  
✔ Controlled access  

---

## ⚠️ Data Quality Challenge

### ❗ Delimiter Issue
Some structured files used `|` instead of `,`

### ✅ Resolution
- Explicit delimiter configuration
- Schema validation before ingestion
- Re-sync after cleanup

---

## 🧠 Outcome

✔ Clean, validated data  
✔ Predictable embeddings  
✔ High-quality retrieval downstream  
