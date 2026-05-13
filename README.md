# 📊 Telco Customer Churn Analysis

This project analyzes a telecommunications dataset to identify key factors contributing to customer churn and provides actionable insights for retention strategies.

## 🚀 Interactive Notebook
GitHub's built-in notebook viewer often fails to render interactive visualizations and can have issues with navigation links. 

To view the **full analysis, interactive Tableau charts, and a functional Table of Contents**, please use the nbviewer link below:

👉 **[View the Full Analysis on nbviewer](https://nbviewer.org/github/Ilana-Movshovich/Telco-Churn-Analysis/blob/main/Telco_Churn_Analysis.ipynb)**

---

## 🛠️ Project Highlights
* **`Exploratory Data Analysis`**: A comprehensive deep dive into customer demographics, geographical distribution, and service usage patterns.
* **`Churn Overview Dashboard`**: A centralized Tableau dashboard providing a high-level view of critical KPIs and churn distribution across various categories like contract type, offer, city, etc.
* **`Key Performance Indicators (KPIs)`**: Detailed tracking and analysis of Churn Rate, Net Customer Change, Estimated MRR, ARPU, and Quarterly Revenue at Risk.
* **`Actionable Insights`**: Identification of high-risk segments, such as customers on Month-to-Month contracts or those influenced by competitor offers.

## 🛠️ Analysis Refinement

I used AI tools (Claude/Gemini) to audit my initial findings and help solve specific analytical gaps:

* **Deeper Churn Insights:**
    * **`The "Neutral" Risk`**: Looked specifically at customers with a **Satisfaction Score of 3**. Identified that those on **Month-to-Month Fiber plans** are the most at-risk, with one specific promotion (**Offer E**) reaching a **69.7% churn rate**.
    * **`Revenue Leakage (CLTV Tiers)`**: Shifted focus from just counting "heads" to calculating the actual **financial impact** across CLTV quartiles. This revealed that while **"Whales" (Top 25% CLTV)** made up only a portion of churners, they were responsible for **32.4% ($1.19M)** of the total revenue lost.
    * **`Fact-Checking Assumptions`**: Proved that **"Senior Churn"** was actually caused by **contract length** and **internet type**, not age.
    * **`Offer Analysis`**: Identified that **Offer E** was likely attracting short-term users who left quickly rather than building long-term loyalty.

* **SQL Optimization:**
    * **`Performance at Scale`**: Rewrote queries to run faster on larger datasets (700k+ rows) by fixing redundant code and improving how the database searches through information (**SARGability**).
    * **`Defensive Coding`**: Added safety checks to prevent errors like **dividing by zero** during calculations.
      
## 📍 Data Source
This project utilizes the **Telco Customer Churn dataset**, originally provided by **IBM**. The dataset consists of 7,043 records representing a fictitious telecommunications company in California.

## 📂 Dataset Information
The analysis is based on multiple datasets reflecting different aspects of customer behavior. All raw data files can be found in the [/dataset](./dataset) folder:

* **`demographics.csv`**: Personal information such as gender, age, and marital status.
* **`services.csv`**: Details on internet types, contract types, tenure lengths, phone services, friend referrals, add-ons, etc.
* **`population.csv`**: Population size per zipcode.
* **`location.csv`**: Details on each city, includig zipcode and coordinates.
* **`churn_status.csv`**: Customer churn status data such as churn status (Yes/No), churn score, CLTV, satisfaction score, churn category and churn reason.

## 🗄️ Repository Contents
* **`Dataset/`**: A dedicated directory containing the 4 raw CSV files used in this analysis (Demographics, Services, Population, and Churn Status).
* **`Telco_Churn_Analysis.ipynb`**: The complete Python analysis, covering data merging, EDA, and visualizations.
* **`Telco_Churn_Presentation.pdf`**: A comprehensive project summary and presentation (in Hebrew) covering the key churn insights.
