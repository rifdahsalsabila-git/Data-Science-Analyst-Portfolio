# Data-Science-Analyst-Portfolio
Hi, I'm Rifdah Salsabila! You can call me Rifdah. I'm a fresh mathematics graduate from University of Indonesia. Currently I have serious interest in Data Analytics and Data Science. I'm also looking for any internship or entry level jobs related to data analytics/data science. This repository showcases my data science and machine learning projects, tracking my progress and skills in the field.

My CV in Bahasa Indonesia: [Click here](https://github.com/rifdahsalsabila-git/Data-Science-Analyst-Portfolio/blob/main/CV_Rifdah%20Salsabila.pdf)

## Table of Contents
- [Portfolio Projects](#portfolio-projects)
  - Python
    - [Mpox Classification](#mpox-classification)
    - [Sentiment Analysis: Valko Removal](#sentiment-analysis-valko-removal)
  - SQL & Power BI
    - [Classic Models Business Sales Analysis](#classic-models-business-sales-analysis)
  - Excel
    - [Bank Customer Churn Analysis](#bank-customer-churn-analysis)
- [Education](#education)
- [Contact](#contact)
  
## Portfolio Projects
In this section I list my data science / machine learning projects, briefly describing the problem, approach, and results.

### Mpox Classification
- **Code:** [`Mpox_Classification.ipynb`](https://github.com/rifdahsalsabila-git/Mpox-Classification)
- **Goal:** To classify patient into positive or negative Mpox based on clinical features and laboratory data.
- **Skills:** data cleaning, exploratory data analysis, feature selection, ensemble modeling, model evaluation.
- **Library:** Python, Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Graphviz.
- **Description:** The dataset contains 500 patient records with 50 raw features covering demographics, clinical symptoms, and lab test results. The project involved data cleaning, exploratory data analysis, manual feature selection (keeping necessary features based on papers), and training a Bagging ensemble model with 50 Decision Trees, validated across 3 random seeds (0, 1, 42) for robustness.
- **Results:** The model achieved an average test accuracy of 98.3% and recall of 99.4% across 3 random seeds. Platelet count emerged as the dominant predictive feature (67% importance), followed by ALT level and sore throat symptoms. Notable finding: although training accuracy reached 100%, the test accuracy doesn't fall off way too far from train accuracy, meaning the model doesn't overfit/underfit. The high accuracy might've been due to the combination of features in the decision tree that could identify a positive/negative patient.
  
### Sentiment Analysis: Valko Removal
- **Code:** [`Sentiment_Analysis_Valko_Removal.ipynb`](https://github.com/rifdahsalsabila-git/Sentiment-Analysis-using-BERTweet)
- **Goal:** To classify public sentiment (Positive/Neutral) toward the Valko character removal controversy in the game Love and Deepspace, based on tweets.
- **Skills:** text preprocessing, exploratory data analysis, transfer learning/fine-tuning, handling class imbalance, model evaluation.
- **Library:** Python, PyTorch, HuggingFace Transformers (BERTweet), Pandas, Scikit-learn, Seaborn, Matplotlib, WordCloud.
- **Description:** The dataset consists of 100 English tweets related to the hashtag #Valko, labeled Positive or Neutral. The project involved EDA (label/language distribution, hashtag & word frequency, wordcloud, emoji analysis), text preprocessing (URL/mention normalization, retweet removal), and fine-tuning BERTweet (a RoBERTa-based model pretrained on Twitter data) for binary sentiment classification, using class weights to handle label imbalance.
- **Results:** The model achieved 90% test accuracy and a weighted F1-score of 0.90, with strong performance on the Positive class (F1 0.94) and reasonable performance on the smaller Neutral class (F1 0.67, based on only 3 test samples). Given the small dataset size (100 tweets), results are promising but would benefit from more data for stronger generalization.
  
### Classic Models Business Sales Analysis
- **Code:** [`ECOMMERCE_DASHBOARD.sql`](https://github.com/rifdahsalsabila-git/Sales-Business-Analytics) and [`ECOMMERCE_DASHBOARD.pbix`](https://github.com/rifdahsalsabila-git/Sales-Business-Analytics)
- **Goal:** To prepare and explore the sales data of a scale-model vehicle retailer using SQL, then build a Power BI dashboard that helps management monitor sales performance and cancellation risk.
- **Skills:** data preprocessing (missing values, duplicates, orphan records, outliers), exploratory data analysis, multi-table joins, SQL views, data validation, DAX measures, dashboard design, data storytelling.
- **Tools:** MySQL, MySQL Workbench, Power BI.
- **Description:** The classicmodels database consists of 8 related tables covering customers, orders, order details, products, product lines, payments, employees, and offices. In SQL, I first ran data quality checks (missing values, duplicates, text consistency, and price outliers), then wrote 21 queries to explore revenue, profit, products, customers, countries, monthly trends, sales reps, order status, cancellations, and shipping performance. The data was then combined into a single view (`vw_sales`) at order-line level and validated against the raw tables. In Power BI, I built a 2-page dashboard: an **Overview** page (KPI cards, sales/profit trend, sales by product line, profit by country, top customers, top sales reps) and an **Insights** page (cancelled value, cancel rate, revenue at risk, order status, cancellations by product line, plus dynamic key insights and a recommendation).
- **Results:** The dataset holds about $9.60M in sales and $3.83M in profit. Around 2% of orders have no shipped date, which turned out to be unshipped orders rather than data errors, so they were kept. Cancelled orders account for about $238.85K, or 2.49% of total sales, and Classic Cars is both the largest product line and the biggest source of cancelled value. Orders still On Hold, In Process, or Disputed represent additional revenue at risk. The dashboard gives management a quick view of what drives revenue and where to follow up, supporting decisions on inventory, key accounts, and order handling.

### Bank Customer Churn Analysis

- **Code:** [`Bank Churn Analysis.xlsx`](https://github.com/rifdahsalsabila-git/Bank-Churn-Analysis-with-Excel)
- **Goal:** To analyze bank customer churn behaviour and identify customer segments that should be prioritized for retention.
- **Skills:** data cleaning, data merging, exploratory data analysis, data visualization, dashboard creation, business analysis.
- **Tools:** Microsoft Excel, XLOOKUP, PivotTable, PivotChart.
- **Description:** The dataset consists of 9,998 bank customer records from two related datasets containing account and customer information. The datasets were merged using Customer ID with XLOOKUP, followed by duplicate removal and additional feature creation for analysis. An Excel dashboard was then created to answer key questions about customer churn, customer segments, and balance lost due to churn.
- **Results:** From 9,997 customers after preprocessing, 2,037 customers churned (20.38%), resulting in approximately €185.6 million in lost balance. Germany had the highest churn rate (32.46%), followed by customers with 1 product (27.73%) and non-active members (26.86%). High-value customers had a 23.10% churn rate and accounted for approximately €71.7 million in lost balance, making them an important segment to prioritize for retention.
  
## Education
`University of Indonesia`:
`Bachelor in Mathematics`
`(2021-2026)`

## Contact
- LinkedIn: `linkedin.com/in/rifdah-salsabila732998218`
- Email: `rifdahdjamaan@gmail.com`
- Phone: `+62-812-1244-1448`
