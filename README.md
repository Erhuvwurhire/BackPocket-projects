
# Project 1: Market Segmentation using Clustering – BackPocket

**Project Type**: Unsupervised Machine Learning  
**Platform**: Google Colab | GitHub  
**Tools**: Python, Pandas, Scikit-learn, Matplotlib, Seaborn

## Project Summary

This project applies **clustering algorithms** to segment customers of **BackPocket**, a gifting recommendation platform that helps users select thoughtful gifts for others based on filled-in profiles (recipient’s hobbies, preferences, past gifts, etc.).

By analyzing historical gift data and user preferences, we aim to discover **natural customer segments** that can power:
- 🎯 Targeted marketing campaigns
- 🛍️ Personalized gift suggestions
- 📈 Better product-store partnerships

---

##  Problem Statement

BackPocket users fill out profiles about the recipients they want to gift. These profiles contain information like:
- Age and relationship to gift recipient
- Occasion and gift history
- Hobbies and favourite items
- Budget and shopping preferences

We seek to group these users into **meaningful clusters** to improve:
- Campaign targeting (e.g., gamers vs. wellness buyers)
- In-app UX personalization
- Store-matching efficiency

---

##  Methods Used

- Synthetic data simulation (to model realistic user behavior)
- Feature encoding (One-hot, label encoding)
- Dimensionality reduction with **PCA**
- Clustering with **K-Means** and **DBSCAN**
- Cluster visualization using **t-SNE** and **PCA 2D plots**
- Cluster profiling (e.g., gift history vs. hobbies)

---
Project Context:
You’re segmenting customers on BackPocket based on purchase history, hobbies, favorite movies, previous gifts, etc., to group them into similar clusters for targeted marketing and recommendations.

 Reasons for using K-Means:
Unsupervised Learning:
with the lack of predefined categories. K-Means helps discover natural groupings (clusters) in the data.

Scalability:
It scales well to large datasets, which is ideal for e-commerce or customer data.

Interpretability:
The cluster centroids give insights into what characterizes each segment (e.g., Movie Lovers, Hobbyists, Last-Minute Shoppers).

Simplicity and Speed:
It’s fast, relatively easy to implement, and provides baseline clustering results that can be improved later.

Why Use PCA Before K-Means?
Problem:
High-dimensional data (e.g., if you encode hobbies, movies, previous gifts, etc.) can cause:

Curse of dimensionality – distances become less meaningful

Sparsity – customer vectors might be mostly zero (e.g., many hobbies not selected)

Slow performance and noisy clusters

 Benefits of PCA:
Dimensionality Reduction:
Reduces data to the most important components (e.g., top 10–20) while retaining most of the variance.

Improves K-Means Performance:

Reduces noise and redundancy

Makes clusters more compact and separable

Visualization:

You can plot clusters in 2D or 3D using top principal components.

## 📊 Features Engineered

| Feature | Description |
|--------|-------------|
| `age` | User age |
| `relationship` | e.g., friend, spouse, co-worker |
| `hobbies` | e.g., tech, books, wellness, cooking |
| `last_gift_category` | e.g., electronics, clothing |
| `occasion` | Birthday, Anniversary, Holiday |
| `budget_range` | Low, Medium, High |
| `store_preference` | Online-only, Boutique, Branded |

---

##  Key Insights

- Clustering revealed 4–5 dominant user personas, including:
  - 🎮 *The Trendy Tech Shopper*
  - 💅 *The Wellness & Self-Care Buyer*
  - 🎁 *The Holiday Generalist*
- Younger users preferred novelty gifts, while older users focused on practical items.
- Seasonal buyers showed significant overlap across multiple hobby types.

---

##  Impact on Business

These customer segments help the BackPocket platform:
- Improve **gift matching logic** via persona-driven filtering.
- Create **marketing campaigns** based on lifestyle & intent.
- Partner with **relevant stores** for high-converting categories.

---

## 📂 Repository Structure
<img width="1144" height="828" alt="image" src="https://github.com/user-attachments/assets/066c0dc7-5684-4013-8894-36aa85b61c77" />

---

##  How to Run

1. Clone this repo  
   `git clone https://github.com/yourusername/backpocket-ml.git`
2. Open the `notebooks/market_segmentation.ipynb` in Google Colab or Jupyter
3. Run all cells to:
   - Generate or load customer data
   - Apply clustering
   - Visualize and interpret clusters

---

## Next Steps

- Integrate with downstream recommender system
- Train classifiers to auto-assign users to segments
- Track segment engagement over time

---

## 📄 License

MIT License. Feel free to use and modify for non-commercial or research purposes.





