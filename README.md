# 🍽️ Restaurant Rating Prediction & Analysis | Cognifyz Internship

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Pandas%20%7C%20Scikit--Learn-orange)
![Tool](https://img.shields.io/badge/Tool-PowerBI%20%7C%20Tableau-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This repository contains the complete coursework and final project for my **Data Science Internship at Cognifyz Technologies**. 

The goal of this project was to analyze a large dataset of **9,500+ restaurants**, clean messy data, perform exploratory data analysis (EDA), and build a machine learning model to **predict aggregate restaurant ratings**.

**Key Outcome:** Built a **Random Forest Regressor** with **96% accuracy (R²)** and created a hybrid interactive dashboard using **Power BI** and **Tableau**.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 🐍
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Plotly Express.
* **BI Tools:** Microsoft Power BI (Dashboarding), Tableau (Geospatial Analysis).
* **Environment:** Google Colab / Jupyter Notebook.

---

## 📂 Project Structure (The 3 Levels)

### 🔹 Level 1: Data Exploration & Preprocessing
**Goal:** Understand the raw data and prepare it for analysis.
* **Data Cleaning:** Handled missing values in the 'Cuisines' column and removed 2,148 'Not Rated' (0.0) entries to prevent skewing.
* **Data Type Conversion:** Converted categorical 'Yes/No' columns into numeric 1/0 values.
* **Geospatial Analysis:** Visualized restaurant locations using **Plotly Express** to identify high-density clusters (e.g., New Delhi).

### 🔹 Level 2: Descriptive Analysis & Feature Engineering
**Goal:** Extract insights and create new features for better model performance.
* **Service Analysis:** Discovered that restaurants with **Table Booking** have significantly higher average ratings than those without.
* **Feature Extraction:** Created new features:
    * `Name Length` & `Address Length`
    * `Cuisine Count` (calculated by "exploding" and counting multi-cuisine strings).
* **Challenge Overcome:** Fixed a critical bug where categorical variables had hidden whitespace (`"Yes "` vs `"Yes"`), which was causing analysis errors. Used `.str.strip()` to resolve.

### 🔹 Level 3: Predictive Modeling & Advanced Visualization (Capstone)
**Goal:** Predict ratings and tell the data story.
* **Machine Learning:** Trained three regression models:
    1.  **Linear Regression:** (R²: ~0.28) - Poor fit for complex data.
    2.  **Decision Tree:** (R²: ~0.91) - Good, but prone to overfitting.
    3.  **Random Forest:** (R²: ~0.96) - **Best Model** with the lowest RMSE (0.30).
* **Customer Preference:** Identified that while *North Indian* cuisine is the most popular by votes, niche cuisines often command higher average ratings.

---

## 📊 Visualizations (Hybrid Approach)

For the final data storytelling, I utilized a **Hybrid BI Approach**:

1.  **Power BI Dashboard:**
    * Used for statistical analysis (Histograms, Box Plots, Correlation Heatmaps).
    * Implemented interactive Slicers for `City` and `Price Range`.
    * [Insert Link to Power BI PDF/Screenshot here]

2.  **Tableau Geospatial Map:**
    * Used specifically for mapping 9,500+ locations.
    * Color-coded by rating and sized by vote volume for immediate visual insights.
    * [Insert Link to Tableau Public/Screenshot here]

---

## 💡 Key Insights
1.  **Price vs. Quality:** There is a strong positive correlation between `Price Range` and `Aggregate Rating`. Expensive restaurants are generally rated higher.
2.  **The "Booking" Effect:** Table booking is a strong indicator of quality; restaurants offering it rarely have poor ratings.
3.  **Location Matters:** High-rated restaurants tend to cluster in specific urban zones, which was visualized clearly in the geospatial analysis.

---

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/YourUsername/Restaurant-Rating-Prediction.git](https://github.com/YourUsername/Restaurant-Rating-Prediction.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn plotly
    ```
3.  Open the `Cognifyz_Internship_Final.ipynb` file in Jupyter or Colab.

---

## 📬 Connect with Me
**Dineshkumar S** *Final Year ECE Student | Aspiring Data Scientist* [www.linkedin.com/in/dineshkumar-s-745b10347] | [dineshkumar53492@gmail.com]

---
*Verified Project for Cognifyz Technologies Data Science Internship.*
