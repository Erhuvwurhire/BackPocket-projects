# BackPocket-projects _ Market Segmentation with Clustering 
# 🎯 Project 1: Market Segmentation using Clustering – BackPocket

**Project Type**: Unsupervised Machine Learning  
**Platform**: Google Colab | GitHub  
**Tools**: Python, Pandas, Scikit-learn, Matplotlib, Seaborn

## 🧠 Project Summary

This project applies **clustering algorithms** to segment customers of **BackPocket**, a gifting recommendation platform that helps users select thoughtful gifts for others based on filled-in profiles (recipient’s hobbies, preferences, past gifts, etc.).

By analyzing historical gift data and user preferences, we aim to discover **natural customer segments** that can power:
- 🎯 Targeted marketing campaigns
- 🛍️ Personalized gift suggestions
- 📈 Better product-store partnerships

---

## 🔍 Problem Statement

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

## 🧰 Methods Used

- Synthetic data simulation (to model realistic user behavior)
- Feature encoding (One-hot, label encoding)
- Dimensionality reduction with **PCA**
- Clustering with **K-Means** and **DBSCAN**
- Cluster visualization using **t-SNE** and **PCA 2D plots**
- Cluster profiling (e.g., gift history vs. hobbies)

---

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

## 📌 Key Insights

- Clustering revealed 4–5 dominant user personas, including:
  - 🎮 *The Trendy Tech Shopper*
  - 💅 *The Wellness & Self-Care Buyer*
  - 🎁 *The Holiday Generalist*
- Younger users preferred novelty gifts, while older users focused on practical items.
- Seasonal buyers showed significant overlap across multiple hobby types.

---

## 💡 Impact on Business

These customer segments help the BackPocket platform:
- Improve **gift matching logic** via persona-driven filtering.
- Create **marketing campaigns** based on lifestyle & intent.
- Partner with **relevant stores** for high-converting categories.

---

## 📂 Repository Structure


