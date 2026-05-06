# DS_Project
🌍 Global Terrorism Analysis & Predictive Modeling (1970 - 2017)
📌 Project Overview
This project performs an end-to-end Exploratory Data Analysis (EDA) and applies Machine Learning to the United Nations Global Terrorism Analysis (UNGTA) dataset. The project transitions from raw data processing to deep analytical insights and finally to predictive modeling, aiming to understand the evolving landscape of global security.

🛠️ Data Science Methodology
1. Data Wrangling & Cleaning
Column Selection: Reduced the dataset from 135 attributes to 14 essential features (Year, Region, Attack Type, Weapon, etc.) to focus on high-impact variables.

Handling Missing Values: * Numerical values (nkill, nwound) were imputed with 0, assuming blanks represent non-lethal/non-injury events.

Categorical values were filled with "Unknown" to maintain data integrity without dropping significant records.

Feature Engineering:

Casualties: Created by summing nkill and nwound.

High Casualty Flag: Created to categorize incidents based on the median impact.

Fatal Attack Flag: Created to distinguish between lethal and non-lethal incidents.

2. Exploratory Data Analysis (EDA)
The analysis follows the UBM (Univariate, Bivariate, and Multivariate) rule with 20 charts:

Univariate Analysis (U)
Yearly Frequency: Visualizing the massive surge in incidents post-2011.

Attack Types: Identifying Bombings as the dominant tactical choice.

Region Distribution: Highlighting the concentration of attacks in the Middle East and South Asia.

Success Rate: Measuring the overall operational effectiveness of global terrorism.

Group WordCloud: Identifying the most prolific perpetrator groups.

Monthly Trends: Investigating seasonality in terrorist activities.

Fatal Attack Proportion: Analyzing the percentage of lethal versus non-lethal events.

Bivariate Analysis (B)
Annual Fatalities: Tracking human impact over decades.

Lethality by Attack Type: Comparing specific tactics against death tolls.

Casualties by Region: Identifying the human cost across different geographies.

Weapon Success Rate: Correlating weapon choice with mission success.

Suicide Attacks over Time: Tracking the rise of high-intensity suicide tactics.

Top 10 Countries: Ranking nations by total fatalities.

Success vs. Casualties: Visualizing the impact distribution of successful vs. failed attempts.

Multivariate Analysis (M)
Correlation Heatmap: Discovering hidden relationships between tactical variables.

Regional Lethality Trends: Observing the geographical "migration" of high-risk zones.

Multi-pane Tactics: Analyzing year, lethality, and success across different attack categories.

Regional Weapon Choice: Identifying tactical specializations in different parts of the world.

High Casualty Distribution: A violin plot analysis of incident intensity over time.

Global Risk Map: A comprehensive strip plot of fatalities by target sector and region.

3. Machine Learning (Predictive Modeling)
We implemented 5 algorithms to predict the Success of an incident based on geographic and tactical features:

Logistic Regression: Baseline binary classification.

Decision Tree: Logic-based flow for tactical splits.

Random Forest: Ensemble method providing high stability and accuracy.

K-Nearest Neighbors (KNN): Classification based on tactical similarity.

Naive Bayes: Probabilistic modeling for large categorical datasets.

📈 Key Visual Insights
Temporal Surge: Terrorist incidents peaked globally between 2014 and 2017.

Tactical Preference: Bombings/Explosions remain the most frequent and successful weapon types.

Targeting: Private Citizens and Property are the most vulnerable sectors.

🚀 How to Run
Ensure you have the Global Terrorism Data.csv file.

Install dependencies:

Bash
pip install pandas numpy matplotlib seaborn scikit-learn wordcloud missingno
Execute the cells in order to perform cleaning, generate charts, and train models.

👨‍💻 Author
Pranjli Singh B.Tech (Computer Science Engineering)

Roll No: 2472116 Doon University

This project was developed for the Data Science Practical, focusing on a structured approach to EDA and Machine Learning.
