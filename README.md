# 📊 Telco Customer Churn Analysis

This project analyzes a telecommunications dataset to identify key factors contributing to customer churn and provides actionable insights for retention strategies.

## 🚀 Interactive Notebook
GitHub's built-in notebook viewer often fails to render interactive visualizations and can have issues with navigation links. 

To view the **full analysis, interactive Tableau charts, and a functional Table of Contents**, please use the nbviewer link below:

👉 **[View the Full Analysis on nbviewer](https://nbviewer.org/github/Ilana-Movshovich/Telco-Churn-Analysis/blob/0a6c5eaac05f280047e7e16026b0a15fc25eede7/Telco-Churn-Analysis.ipynb)**

---

## 🛠️ Project Highlights
* **`Exploratory Data Analysis`**: A comprehensive deep dive into customer demographics, geographical distribution, and service usage patterns.
* **`Churn Overview Dashboard`**: A centralized Tableau dashboard providing a high-level view of critical KPIs and churn distribution across various categories like contract type, offer, city, etc.
* **`Key Performance Indicators (KPIs)`**: Detailed tracking and analysis of Churn Rate, Net Customer Change, Estimated MRR, ARPU, and Quarterly Revenue at Risk.
* **`Actionable Insights`**: Identification of high-risk segments, such as customers on Month-to-Month contracts or those influenced by competitor offers.

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
* **`Telco_Churn_Presentation.pptx`**: A comprehensive project summary and presentation (in Hebrew) covering the key churn insights.
* **`README.md`**: Project overview, data dictionary, and navigation guide.
