# marketing_analytics_ai_project
Objectives: To apply data science tools for customer segmentation and prediction in marketing.


1️⃣ data/

Place your raw dataset here (you already have tata_online_retail.csv).

This folder only contains raw CSV files or any other raw datasets.

Do not modify the raw CSV directly—always work on a copy in your notebooks.

2️⃣ notebooks/

This is where all your Jupyter notebooks will go, divided by tasks:

01_EDA_and_Segmentation.ipynb

Purpose: Explore the dataset, clean it, and perform customer segmentation.

Steps inside the notebook:

Import libraries (pandas, numpy, matplotlib, seaborn, sklearn).

Load CSV from ../data/tata_online_retail.csv.

Quick exploration: data.head(), data.info(), data.describe().

Data cleaning:

Handle missing values (CustomerID, Description).

Convert InvoiceDate to datetime.

Remove canceled invoices if needed (InvoiceNo starting with 'C').

Feature engineering:

Create TotalPrice = Quantity * UnitPrice.

Aggregate data per customer for segmentation.

Customer segmentation using clustering (KMeans).

Save visuals in ../visuals/ (optional: plt.savefig("../visuals/customer_segmentation.png")).

02_Sales_Forecasting.ipynb

Purpose: Predict future sales using AI/ML.

Steps inside the notebook:

Aggregate sales by date (daily/weekly/monthly).

Handle missing dates or gaps.

Use time series models:

ExponentialSmoothing (Holt-Winters)

Optional: ARIMA/Prophet

Visualize actual vs predicted sales.

Save forecast plots in ../visuals/.

03_Sentiment_Analysis.ipynb

Purpose: Analyze customer reviews or social media sentiment.

Steps inside the notebook:

Collect text data (reviews, tweets, etc.).

Clean text (remove stopwords, punctuation).

Use sentiment analysis libraries:

TextBlob or VADER for quick sentiment scoring.

Optional: Fine-tuned ML/NLP models for deeper insights.

Visualize sentiment distributions.

Save sentiment plots in ../visuals/.

3️⃣ visuals/

Save all charts, plots, and graphs here.

Example filenames:

customer_segmentation.png

sales_forecast_plot.png

sentiment_distribution.png

4️⃣ reports/

Store your final project report here.

Include:

Executive summary

Methodology

Key findings

Visuals (link to visuals/)

Recommendations