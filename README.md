# 🌍 Global Terrorism Analysis & Predictive Modeling (1970 - 2017)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/ML-Classification-green)
![Data Science](https://img.shields.io/badge/Focus-EDA%20%26%20Modeling-orange)

## 📌 Project Overview
This project performs an end-to-end **Exploratory Data Analysis (EDA)** and applies **Machine Learning** to the Global Terrorism Database. The study transitions from raw data processing to deep analytical insights and predictive modeling, aiming to understand the evolving landscape of global security.

---

## 🛠️ Data Science Methodology

### 1. Data Wrangling & Cleaning
*   **Column Selection:** Reduced the dataset from 135 attributes to **14 essential features** (Year, Region, Attack Type, Weapon, etc.) to focus on high-impact variables.
*   **Handling Missing Values:**
    *   *Numerical (nkill, nwound):* Imputed with `0`, assuming blanks represent non-lethal/non-injury events.
    *   *Categorical:* Filled with `"Unknown"` to maintain data integrity without dropping significant records.
*   **Feature Engineering:**
    *   `Casualties`: Created by summing `nkill` and `nwound`.
    *   `High Casualty Flag`: Categorized incidents based on the median impact.
    *   `Fatal Attack Flag`: Distinguished between lethal and non-lethal incidents.

### 2. Exploratory Data Analysis (EDA)
The analysis follows the **UBM (Univariate, Bivariate, and Multivariate)** rule, featuring over 20 visualizations:

#### **Univariate Analysis (U)**
*   **Yearly Frequency:** Visualizing the massive surge in incidents post-2011.
*   **Attack Types:** Identifying Bombings as the dominant tactical choice.
*   **Region Distribution:** Highlighting concentration in the Middle East and South Asia.
*   **Success Rate:** Measuring overall operational effectiveness.
*   **Group WordCloud:** Identifying the most prolific perpetrator groups.

#### **Bivariate Analysis (B)**
*   **Annual Fatalities:** Tracking human impact over decades.
*   **Lethality by Attack Type:** Comparing specific tactics against death tolls.
*   **Weapon Success Rate:** Correlating weapon choice with mission success.
*   **Suicide Attacks:** Tracking the rise of high-intensity suicide tactics.

#### **Multivariate Analysis (M)**
*   **Correlation Heatmap:** Discovering hidden relationships between tactical variables.
*   **Regional Lethality Trends:** Observing geographical "migration" of high-risk zones.
*   **Global Risk Map:** A comprehensive strip plot of fatalities by target sector and region.

### 3. Machine Learning (Predictive Modeling)
We implemented **5 algorithms** to predict the **Success** of an incident based on geographic and tactical features:
1.  **Logistic Regression:** Baseline binary classification.
2.  **Decision Tree:** Logic-based flow for tactical splits.
3.  **Random Forest:** Ensemble method providing high stability and accuracy.
4.  **K-Nearest Neighbors (KNN):** Classification based on tactical similarity.
5.  **Naive Bayes:** Probabilistic modeling for large categorical datasets.

---

## 📈 Key Visual Insights
*   **Temporal Surge:** Terrorist incidents peaked globally between 2014 and 2017.
*   **Tactical Preference:** Bombings/Explosions remain the most frequent and successful weapon types.
*   **Targeting:** Private Citizens and Property are the most vulnerable sectors.

---

## 🚀 How to Run

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/YourUsername/DS_Project.git](https://github.com/YourUsername/DS_Project.git)
    ```

2.  **Install Dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn wordcloud missingno
    ```

3.  **Data Setup:**
    Ensure the `Global Terrorism Data.csv` file is placed in the root directory.

4.  **Execution:**
    Run the Jupyter Notebook or Python script to perform cleaning, generate charts, and train models.

---

## 👨‍💻 Author
**Pranjli Singh**
*   *B.Tech (Computer Science Engineering)*
*   *Roll No: 2472116*
*   *Doon University*

---
> This project was developed for the **Data Science Practical**, focusing on a structured approach to EDA and Machine Learning.
