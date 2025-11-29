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

DEMO DASHBOARD ANALYSIS:
<img width="1301" height="739" alt="Screenshot 2025-11-29 103657" src="https://github.com/user-attachments/assets/b5c8b68f-1992-4f73-ae36-ee9ce6bcd4da" />
<img width="1302" height="745" alt="Screenshot 2025-11-29 103729" src="https://github.com/user-attachments/assets/4ab75f47-f8f5-4d93-b9f8-8f8745cda4c1" />
<img width="1297" height="744" alt="Screenshot 2025-11-29 103752" src="https://github.com/user-attachments/assets/825d7a91-bd94-47ba-910a-d797ea4809ab" />
<img width="1295" height="742" alt="Screenshot 2025-11-29 103853" src="https://github.com/user-attachments/assets/a8f692ca-c53f-4540-9f77-a47d0022e783" />
<img width="1786" height="1077" alt="Screenshot 2025-11-29 104101" src="https://github.com/user-attachments/assets/b3df5d5c-a478-4a87-8299-7e523fbd8d2a" />
<img width="1800" height="1079" alt="Screenshot 2025-11-29 104131" src="https://github.com/user-attachments/assets/c13cfe73-9fde-4e68-afc3-9e37dc039fbe" />
<img width="1799" height="1079" alt="Screenshot 2025-11-29 104140" src="https://github.com/user-attachments/assets/37a2eb28-d4c9-4ca8-a989-f9c7e904daa6" />

