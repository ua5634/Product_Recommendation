# Product_Recommendation# ProRec: Product Recommendation System

## 📌 Project Overview
ProRec is a **Product Recommendation System** built using **collaborative filtering** and **content-based filtering**. It analyzes user interactions, product metadata, and ratings to provide personalized product recommendations.

## 🚀 Features
- **Content-Based Filtering:** Recommends products based on product descriptions, categories, and brand similarities using TF-IDF and cosine similarity.
- **Collaborative Filtering:** Suggests products based on similar users' preferences.
- **Hybrid Recommendations:** Combines both content-based and collaborative filtering for better recommendations.
- **Data Cleaning & Preprocessing:** Handles missing values, removes duplicates, and standardizes text data.
- **Visualizations:** Generates heatmaps and bar plots for better insights into product interactions.

## 🛠 Tech Stack
- **Python** (Core language)
- **Pandas & NumPy** (Data handling & manipulation)
- **Matplotlib & Seaborn** (Data visualization)
- **Scikit-learn** (Machine learning models & similarity calculations)
- **SpaCy** (Text preprocessing & stopword removal)
- **TF-IDF Vectorizer** (Text feature extraction)
- **Cosine Similarity** (Similarity measure for recommendations)

## 📂 Dataset Used
The project uses a Walmart product dataset containing:
- **Product ID, Name, Brand, Category**
- **Product Rating & Reviews**
- **Product Description & Tags**

## 🔧 Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ProRec.git
   cd ProRec
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn spacy
   ```
3. Download SpaCy language model:
   ```bash
   python -m spacy download en_core_web_sm
   ```
4. Run the Jupyter Notebook or Python script to generate recommendations.

## 🎯 Usage
### 1️⃣ Content-Based Filtering
```python
from recommendation import content_based_recommendations
item_name = "OPI Nail Lacquer"
content_recs = content_based_recommendations(train_data, item_name, top_n=5)
print(content_recs)
```

### 2️⃣ Collaborative Filtering
```python
from recommendation import collaborative_filtering_recommendations
target_user_id = 4
collab_recs = collaborative_filtering_recommendations(train_data, target_user_id, top_n=5)
print(collab_recs)
```

### 3️⃣ Hybrid Recommendations
```python
from recommendation import hybrid_recommendations
hybrid_recs = hybrid_recommendations(train_data, target_user_id, item_name, top_n=5)
print(hybrid_recs)
```

## 📊 Visualizations
- **Heatmaps** for rating distributions.
- **Popular Items Bar Charts** for trending products.
- **User Interaction Histograms** to analyze engagement.

## 💡 Future Enhancements
- Deploy as a **REST API** for real-time recommendations.
- Improve **collaborative filtering** using deep learning (Neural Networks).
- Implement **user-based recommendations** with demographic filtering.

## 📜 License
This project is open-source and available under the **MIT License**.

## 📞 Contact
For any queries or contributions, reach out via [GitHub Issues](https://github.com/yourusername/ProRec/issues).

---
🔗 **GitHub Repository**: [ProRec](https://github.com/yourusername/ProRec)
