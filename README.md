# 💳 Credit Card Clustering App

This project demonstrates how to use **K-Means clustering** to segment credit card users based on their financial behavior. The clustering is performed using three key features: **BALANCE**, **PURCHASES**, and **CREDIT_LIMIT**. By grouping users into clusters, banks and financial institutions can gain insights into customer spending patterns, identify high-value clients, and design targeted marketing strategies.

## 🧠 Objective
The main goal of this project is to create a simple yet effective machine learning model that can predict which cluster a new credit card user belongs to. This helps in understanding different types of customers based on their financial activity.

## ⚙️ Methodology
1. **Data Preparation**  
   - Only numerical columns (`BALANCE`, `PURCHASES`, `CREDIT_LIMIT`) are used.  
   - Missing values are filled with the median.  
   - Data is scaled using **Min-Max Scaler** to bring values to the range [0,1].

2. **Model Training**  
   - **K-Means** clustering is applied with `n_clusters=5`.  
   - The trained model is saved using **Joblib** for future predictions.

3. **Prediction & Deployment**  
   - A minimal **Streamlit app** allows users to input the three features.  
   - The app scales the input, predicts the cluster, and displays it instantly.

## 📊 Features
- Interactive **Streamlit interface** for entering user data.
- **Cluster predictions** for new users in real-time.
- Easy-to-understand **3-feature model** for quick deployment.
- Saved **model and scaler** using Joblib for reproducibility.

