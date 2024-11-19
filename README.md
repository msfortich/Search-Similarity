
# **Search Term Similarity Project**

## **Project Overview**
The **Search Term Similarity Project** is a data-driven initiative designed to analyze Amazon's monthly search query data. By leveraging cosine similarity, this project links emerging search terms to broader market trends, providing actionable insights for targeted strategies across departments such as Marketing, Sales, and Product Development. Results are automatically ingested into Google BigQuery for continuous analysis and scalability.

---

## **Key Objectives**
1. **Trend Discovery**: Analyze Amazon search queries to identify emerging trends and patterns.
2. **Semantic Relationship Mapping**: Use cosine similarity to discover relationships between new and existing search terms.
3. **Automation**: Streamline the integration of results into BigQuery for continuous monitoring and analysis.
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
- **Tools**: Python's `scikit-learn` library for vectorization and similarity computation.

### **3. Data Integration**
- **Output**: Structured tabular results containing:
  - Search term pairs.
  - Similarity scores.
  - Mapped trend categories.
- **BigQuery Integration**:
  - Automated ingestion of results into BigQuery for centralized storage and ongoing analysis.

### **4. Trend Analysis**
- Linked search terms with broader market trends.
- Grouped related terms to provide actionable insights.

---

## **Technologies & Tools**
- **Programming Language**: Python
- **Libraries**:
  - `pandas` and `numpy` for data manipulation.
  - `scikit-learn` for TF-IDF vectorization and cosine similarity.
- **Cloud Platform**: Google Cloud Platform (BigQuery)
- **Collaboration Tools**: GitHub for version control and team collaboration.

---

## **Results**
- Established a scalable pipeline to process monthly search data.
- Automated ingestion of similarity results into BigQuery, ensuring continuous trend monitoring.
- Delivered actionable insights that inform marketing strategies, improve product positioning, and drive consumer engagement.

---

## **How to Use**

### **Setup**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name/search-term-similarity.git
   cd search-term-similarity
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### **Execution**
1. Preprocess data:
   ```bash
   python preprocess.py
   ```
2. Run the similarity analysis:
   ```bash
   python compute_similarity.py
   ```
3. Export results to BigQuery:
   ```bash
   python export_to_bigquery.py
   ```

---

## **Example Output**
| Term 1        | Term 2         | Cosine Similarity | Trend Category |
|----------------|----------------|-------------------|----------------|
| "wireless mouse" | "bluetooth mouse" | 0.89              | Electronics    |
| "diet shakes"   | "protein drinks"   | 0.85              | Health         |

---

## **Future Enhancements**
1. **Explore Advanced Models**: Implement deep learning approaches like Word2Vec or BERT for improved semantic similarity.
2. **Interactive Visualization**: Develop dashboards to visualize trends in real-time.
3. **Additional Metrics**: Incorporate other similarity measures like Jaccard similarity for richer insights.

---

## **Contributors**
- **Madi Fortich**: Project Lead and Developer
- **Data Science Team**: Provided support with modeling and analysis.
- **Metadata Team**: Shared domain knowledge and search query datasets.

---
