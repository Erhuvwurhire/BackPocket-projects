# BackPocket-projects
# 🎁 Personalized Gift Recommendation Engine (Project 1) 

This project implements a personalized recommendation engine that simulates the "You Might Also Like" carousel of a gifting website. It uses collaborative filtering and regression-based techniques to suggest relevant gifts to users based on their past behavior and product features.

## 🚀 Project Overview

**Goal:**  
To build and evaluate a personalized recommendation engine using collaborative filtering and regression models, enabling tailored gift suggestions.

**Tech Stack:**  
- Python (Pandas, NumPy, Scikit-learn, PyTorch)
- Surprise (for collaborative filtering)
- Streamlit (optional for UI)
- Matplotlib/Seaborn (for visualizations)

## 📊 Problem Statement

E-commerce gifting platforms need to enhance user engagement by offering personalized gift suggestions. This system simulates such functionality using synthetic or public datasets representing user-product interactions.

## 🔍 Key Features

- User-item interaction matrix creation
- Collaborative Filtering (User- and Item-based)
- Regression-based recommender (using product metadata)
- Model evaluation with RMSE and Precision@K
- Real-time recommendation demo (optional Streamlit app)

## 📁 Project Structure

gift-recommender-ml/
│
├── data/ # Sample or synthetic datasets
│ └── user_product.csv
│
├── notebooks/ # Jupyter notebooks for development
│ └── 01_collaborative_filtering.ipynb
│ └── 02_regression_model.ipynb
│
├── src/ # Python scripts (modular code)
│ ├── recommender.py
│ └── utils.py
│
├── app/ # Optional: Streamlit app for demo
│ └── app.py
│
├── requirements.txt # Required Python packages
├── README.md # Project documentation
└── LICENSE



## 🧠 How It Works

### Collaborative Filtering

- Based on the user-item interaction matrix
- Implemented using K-Nearest Neighbors (KNN) from Surprise library
- Recommends items liked by similar users

### Regression-Based Model

- Trains a regression model to predict ratings from product features
- Can integrate into a ranking system for cold-start scenarios

## ✅ Evaluation

| Model                | RMSE  | Precision@5 |
|---------------------|-------|-------------|
| Collaborative (User) | 0.92  | 0.64        |
| Regression           | 1.04  | 0.58        |

> (Replace the above table with your actual results after training)

## 🖥️ Optional: Streamlit App

Run the app with:

```bash
cd app
streamlit run app.py
