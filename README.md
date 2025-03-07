# **Decoding AI Impact in News Articles using NLP**

## **Overview**
This project applies Natural Language Processing (NLP) techniques to analyze nearly 200,000 news articles related to Artificial Intelligence (AI), Machine Learning, and Data Science between 2020 and 2024. The analysis identifies industries and job roles most impacted by AI, uncovers sentiment trends, and highlights key players driving AI innovation.

---

## **Business Problem**
Understanding how AI technologies reshape industries and occupations is critical for strategic planning. This project addresses the need to:
- Identify which industries will benefit or be disrupted by AI.
- Recognize job roles with increasing demand or at risk due to AI.
- Assess public sentiment toward AI advancements.
- Discover influential organizations and individuals in the AI field.
- Offer actionable insights for stakeholders to leverage AI effectively.

---

## **Dataset and Features**

### **Dataset Overview**
- **Source**: News articles from multiple outlets (2020-2024)
- **Size**: ~200,435 articles (900 MB, Parquet format)
- **Topics Covered**:
  - AI Innovation
  - Machine Learning
  - Data Science

### **Data Preparation**
- **Filtering**: Selected articles mentioning AI-related keywords.
- **Cleaning**: Removed irrelevant content (URLs, HTML tags, emails, special characters, stopwords).
- **Text Normalization**: Applied tokenization and lemmatization.
- **Duplicates**: Eliminated duplicate articles.

---

## **Methodology**

### **Topic Modeling**
- **Technique**: Latent Dirichlet Allocation (LDA) using Gensim.
- **Approach**: Included bi-grams and tri-grams for topic coherence.
- **Result**: Identified 14 distinct topics categorized into 5 main groups:
  - AI Technology & Innovation
  - Business Solutions
  - Finance & Markets
  - Healthcare
  - News & Media

### **Sentiment Analysis**
- **Tool**: VADER (Valence Aware Dictionary and sEntiment Reasoner)
- **Classification**:
  - Positive sentiment: ≥ 0.5
  - Neutral sentiment: -0.5 to 0.5
  - Negative sentiment: ≤ -0.5
- **Outcome**: Majority of articles expressed positive or neutral sentiments towards AI.

### **Named Entity Recognition (NER)**
- **Tool**: SpaCy
- **Purpose**: Extracted frequently mentioned companies and individuals.
- **Highlighted Entities**:
  - **Organizations**: Microsoft, Google, Amazon, IBM, Apple
  - **Individuals**: Elon Musk (Tesla, Neuralink), Sam Altman (OpenAI)

---

## **Key Findings**

### **Industries Positively Impacted**
- Healthcare
- Science Research
- Education

### **Industries Negatively Impacted**
- Energy
- Government
- Public Services

### **Job Market Insights**
- **High-demand Jobs**:
  - Data Scientist
  - Software Engineer
- **At-risk Jobs**:
  - Architect
  - Pilot
  - Tutor

---

## **Recommendations**
- **Innovation Leadership**: Support leaders driving AI advancements, such as Elon Musk and Sam Altman.
- **Collaborative Ecosystem**: Promote partnerships between tech giants, academic institutions, and governments.
- **Educational Alignment**: Focus education on skills relevant to emerging AI-related roles.
- **Ethical AI**: Develop and adhere to ethical standards to manage societal impacts.

---

## **Visualizations**
- **Topic Analysis**: Distribution of articles across AI-related topics.
- **Sentiment Trends**: Analysis of sentiment evolution over time.
- **Entity Prominence**: Visual representation of influential entities.

---

## **Tools & Technologies Used**
- **Programming Language**: Python
- **Libraries**: SpaCy, Gensim, VADER, Pandas, NumPy
- **Visualization**: Matplotlib

---

## **Results Summary**

| **Category**                 | **Details**                                 |
|------------------------------|---------------------------------------------|
| **Industries Benefiting**    | Healthcare, Science Research, Education     |
| **Industries at Risk**       | Energy, Government, Public Services         |
| **Jobs in Demand**           | Data Scientist, Software Engineer           |
| **Jobs at Risk**             | Architect, Pilot, Tutor                     |
| **Key Companies**            | Microsoft, Google                           |
| **Influential Individuals**  | Elon Musk, Sam Altman                       |
| **Dominant Sentiment**       | Positive & Neutral                          |

---

## **Limitations & Future Work**

### **Limitations**
- Sentiment classification may be subjective due to inherent biases in news reporting.
- Results may vary across different data sources or contexts.

### **Future Directions**
- Expand dataset diversity for broader applicability.
- Utilize advanced transformer models (e.g., BERT) for enhanced accuracy.
- Implement continuous, real-time AI impact monitoring.

---

