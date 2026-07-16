# 🛒 E-Commerce Analytics & Recommendation System

## 📝 About The Project
This project is an end-to-end analytics system designed to understand customer behavior, predict purchasing patterns, and generate product recommendations[cite: 2]. It transforms raw data into meaningful business insights by integrating a data warehouse, machine learning pipelines, and an interactive business intelligence dashboard[cite: 2].

📄 **Full Research Paper:** [Read the detailed paper here](./Ecommerce_Recommendation_Paper.pdf)

## 🏗️ System Architecture & Pipeline
The system is built on four interlocking components[cite: 2]:

*   **1. Data Warehouse (DWH):** Constructed in PostgreSQL 18 following a Medallion Architecture (Bronze, Silver, Gold) and structured into a star-schema design[cite: 2].
*   **2. Market Basket Analysis:** Utilizes the FP-Growth algorithm applied to 6,050 unique invoices to extract 1,902 frequent itemsets and identify cross-selling opportunities[cite: 2].
*   **3. Customer Segmentation:** Applies MiniBatch K-Means clustering on Recency-Frequency-Monetary (RFM) features to segment the customer base into distinct behavioral profiles[cite: 2].
*   **4. Value Prediction:** Uses a Logistic Regression model for customer value prediction, achieving an overall accuracy of 93.55% and an AUC of 0.9885[cite: 2].

## 📊 Dataset & Business Impact
The data ingestion and transformation process resulted in a highly refined Gold layer[cite: 2]. The database encompasses:
*   158,050 clean transaction line items[cite: 2].
*   4,338 unique customers[cite: 2].
*   3,921 distinct products[cite: 2].
*   38 countries across five continents[cite: 2].
*   A total generated revenue of £3,122,766.93[cite: 2].

## 📈 Business Intelligence Dashboard
All insights are surfaced through an interactive Power BI dashboard connected in real time to the PostgreSQL Gold layer[cite: 2]. This enables non-technical stakeholders to explore[cite: 2]:
*   Platform performance macro diagnostics[cite: 2].
*   Granular customer behavioral insights[cite: 2].
*   Spatial and regional demographics[cite: 2].

## 📂 Repository Structure
*   `Ecommerce_Analytics_Pipeline.ipynb`: The main notebook containing the ML models (FP-Growth, K-Means, Logistic Regression).
*   `Architecture_and_Data/`: Contains the Star Schema architecture diagram and dataset samples.
*   `PowerBI_Dashboard/`: Contains the source files for the interactive dashboard and screenshots of the different analytical views.
