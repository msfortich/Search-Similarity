
# **Search Term Similarity Project**

## **Project Overview**
The **Search Term Similarity Project** is designed to analyze Amazon's monthly search query data. By leveraging cosine similarity, this project links emerging search terms to broader market trends, providing actionable insights for targeted strategies across departments.
---

## **Key Objectives**
1. **Trend Discovery**: Analyze Amazon search queries to identify emerging trends and patterns.
2. **Semantic Relationship Mapping**: Use cosine similarity to discover relationships between new and existing search terms.
4. **Business Insights**: Support cross-departmental strategies with deeper insights into consumer behavior.

---

## **Methodology**

### **1. Data Collection & Preparation**
- **Source**: Monthly Amazon search query logs.
- **Preprocessing**:
  - Cleaned and normalized search queries (lowercasing, punctuation removal, etc.).
  - Tokenized text data and generated Term Frequency-Inverse Document Frequency (TF-IDF) vectors.

### **2. Cosine Similarity Analysis**
- **Goal**: Measure semantic similarity between search terms.
- **Steps**:
  - Constructed a TF-IDF matrix to represent search terms numerically.
  - Calculated cosine similarity scores to link new search terms with existing trends.

### **3. Data Integration**
- **Output**: Structured csv results containing:
  - Search term pairs.
  - Similarity scores.
  - Mapped trend categories.


### **4. Trend Analysis**
- Linked search terms with broader market trends.
- Grouped related terms to provide actionable insights.

---

## **Results**
- Established a scalable pipeline to process monthly search data for them to be use the output and create an automated ingestion into BigQuery, ensuring continuous trend monitoring.

---

## **Example Output**
| Term 1        | Term 2         | Cosine Similarity | Trend Category |
|----------------|----------------|-------------------|----------------|
| "wireless mouse" | "bluetooth mouse" | 0.89              | Electronics    |
| "diet shakes"   | "protein drinks"   | 0.85              | Health         |
