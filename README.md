# Clustering-of-customer-reviews-for-marketing-insights-using-KMeans


This project applies unsupervised machine learning to analyze and segment Amazon customers based on their review behavior. By using KMeans clustering on structured features derived from customer reviews, the project uncovers distinct customer personas to support targeted marketing strategies.


##  Overview

Traditional market segmentation often ignores rich behavioral cues embedded in customer reviews. This project leverages review-based features—like helpfulness, length, and sentiment indicators—to cluster customers and extract actionable insights.

Key Features:
- Cleaned and preprocessed real-world Amazon product review dataset
- Feature engineering for engagement and sentiment proxies
- KMeans clustering with evaluation metrics (Silhouette Score, CH Index)
- Cluster interpretation for marketing strategy formulation
- Visualizations for cluster quality and insights


---

##  Dataset

- **Source**: Amazon product review dataset (843 records × 19 features after cleaning)
- **Key Fields**: `reviews.text`, `reviews.rating`, `reviews.numHelpful`, `brand`, `name`, `reviews.date`
- **Target Features for Clustering**:
  - `review_length`, `word_count`, `is_helpful`, `rating_deviation`, `engagement_score`, etc.

---

## 🧠 Methods Used

- **Language**: Python
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `nltk`, `textblob`

### ✅ Workflow:

1. **Data Cleaning** (`data_clearing.ipynb`)
   - Handle missing values
   - Drop irrelevant fields
   - Standardize and transform data

2. **Feature Engineering & Clustering** (`review_clustering_kmeans.ipynb`)
   - Extract behavioral features from review data
   - Apply `StandardScaler` for normalization
   - Perform `KMeans` clustering (optimal k selected via Silhouette)
   - Evaluate clusters using:
     - Silhouette Score
     - Calinski-Harabasz Index
     - Elbow Method

3. **Cluster Profiling & Marketing Insights**
   - Generate behavioral summaries per cluster
   - Visualize with bar charts, scatterplots, and heatmaps
   - Recommend tailored strategies (advocacy, retention, engagement)

---

## Sample Insights

- **Cluster 1**: High-rating, short reviews — loyal but brief customers
- **Cluster 4**: Long, detailed reviews with low ratings — critical, high-engagement users
- **Cluster 7**: Highly helpful reviews with high ratings — potential brand advocates

---

## Results

| Metric               | Value     |
|----------------------|-----------|
| Optimal Clusters (k) | 9         |
| Silhouette Score     | 0.398     |
| CH Index             | 283.66    |

---

## Marketing Applications

- **Retention Programs** for dissatisfied clusters
- **Advocacy Campaigns** for helpful, high-rating users
- **Re-engagement Tactics** for low-engagement but loyal reviewers

---

## Getting Started


