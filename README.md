# 🚀 Cryptocurrency Web Scraping & Data Processing Project

## 📌 Project Overview

This project is an end-to-end data pipeline built to **collect, process, analyze, and model cryptocurrency market data**.
The goal is to demonstrate real-world data engineering and data science skills — from raw web data to machine-learning-driven insights.

The project follows a structured workflow:
**Web Scraping → Data Cleaning → Database Storage → Visualization → Feature Engineering → Machine Learning**

---

## 🎯 Objectives

* Scrape real-world cryptocurrency market data from the web
* Clean and normalize noisy, unstructured data
* Store structured data in a relational database
* Build dashboards to analyze market behavior
* Engineer meaningful features for modeling
* Train and evaluate multiple machine learning models
* Predict cryptocurrency price movement (UP / DOWN)

---

## 🌐 Data Collection (Web Scraping)

* Source: **CoinMarketCap**
* Tooling: `requests`, `BeautifulSoup`
* Extracted information includes:

  * Cryptocurrency name
  * Market price
  * Market capitalization
  * Trading volume
  * Percentage changes (daily / weekly)
  * Market dominance

Scraped data is saved as CSV files for reproducibility.

---

## 🧹 Data Cleaning & Processing

Key preprocessing steps:

* Removed missing and inconsistent values
* Converted numeric fields from strings to proper data types
* Handled outliers and invalid entries
* Normalized column names
* Removed duplicates
* Ensured time-series consistency

Cleaned datasets are saved for downstream tasks.

---

## 🗄 Database Storage

* Database: **SQLite**
* Stored cleaned data in structured tables
* Enables efficient querying and visualization
* Keeps raw and processed data separate

---

## 📊 Data Visualization & Dashboard

* Created visual dashboards to explore:

  * Price trends
  * Market dominance
  * Trading volume patterns
  * Cryptocurrency performance over time
* Dashboards help answer questions such as:

  * Which assets dominate the market?
  * How volatile is the market?
  * What trends are emerging?

---

## 🧠 Feature Engineering

Engineered features include:

* Price momentum indicators
* Market dominance ratios
* Percentage price change signals
* Binary target variable (Price Movement: UP / DOWN)

These features improve model learning and prediction quality.

---

## 🤖 Machine Learning Models

Trained and evaluated **5 different models**:

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)
* Gradient Boosting

### 🏆 Best Model

* **Gradient Boosting**
* Achieved ~**95% accuracy**
* Provided the best balance between bias and variance

Model evaluation used:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

The best model is saved for reuse.

---

## 📂 Project Structure

```
WebScraping_and_Data_Processing_Project/
│
├── 01_web_scraping.ipynb
├── 02_saving_data_into_db.ipynb
├── 03_data_visualization
├── 04_data_preprocessing_feature_engineering.ipynb
├── 05_modelling_evaluation.ipynb
│
├── Webscraping_and_Data_Processing_Project.ppt
├── requirements.txt
├── architecture.md
│
├── data/
│   ├── raw_data.csv
│   ├── cleaned_data.csv
│   └── database.db
│
├── models/
│   └── best_model.pkl
│
└── README.md
```

---

## 🛠 Tools & Technologies

* Python
* Pandas
* BeautifulSoup
* Requests
* SQLite
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📈 Key Learnings

* Handling real-world messy web data
* Designing scalable data pipelines
* Feature engineering for financial data
* Comparing multiple ML models objectively
* Translating data into actionable insights
