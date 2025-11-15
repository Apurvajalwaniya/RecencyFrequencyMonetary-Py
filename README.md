# RFM Analysis for Customer Segmentation

This project implements an end-to-end RFM (Recency, Frequency, Monetary) analysis to segment customers based on their purchasing behaviour.  
The goal is to identify high-value users, declining customers, and potential growth segments so businesses can take targeted actions in marketing, retention, and customer lifetime value (CLV) improvement.

---

##  Project Overview

Understanding customer behaviour is critical for any business that depends on repeat purchases.  
This project uses historical transaction data to compute Recency, Frequency, and Monetary metrics for each customer and assigns an RFM score to group users into meaningful segments.

The workflow includes:

- Cleaning and structuring transactional data  
- Computing RFM metrics for every customer  
- Applying quantile-based scoring for R, F, and M  
- Generating combined RFM scores  
- Creating customer segments using score patterns  
- Visualizing spending patterns and behavioural trends  
- Interpreting segment-wise insights for decision-making  

---

##  Dataset Description

The dataset contains individual customer transactions, including:

- **Customer ID**  
- **Invoice Date / Timestamp**  
- **Invoice Number**  
- **Purchase Value**  
- **Quantity / Number of items**  

If your dataset has different column names (e.g., “total_amount”, “order_date”), adjust the notebook accordingly.

---

##  Technologies and Tools Used

- **Python 3.x**
- **Pandas** for data manipulation  
- **NumPy** for numerical operations  
- **Matplotlib & Seaborn** for visualizations  
- **Jupyter Notebook** for analysis and documentation  

These libraries support efficient preprocessing, scoring, and visualization of customer clusters.

---

##  Methodology (Step-by-Step)

### 1. Data Preprocessing
- Checked missing values  
- Removed invalid or negative transactions  
- Converted date columns to proper datetime format  
- Aggregated transaction-level data into customer-level metrics  

### 2. Feature Creation
- **Recency**: Days since last purchase  
- **Frequency**: Total number of purchases  
- **Monetary**: Total spending by each customer  

### 3. Scoring
- Assigned 1–5 scores to each R, F, M metric using quantiles  
- Higher scores indicate more valuable behaviour  

### 4. RFM Score Calculation
- Combined the three scores into a single RFM code (e.g., 555, 431, 222)  
- Mapped these codes to labelled segments  

### 5. Segmentation
Some example groups:

- **Champions** – Very recent, frequent, high-spending customers  
- **Loyal Customers** – Buy often and frequently  
- **Potential Loyalists** – Recent buyers with growing frequency  
- **At-Risk** – Previously good customers with declining activity  
- **Hibernating** – Very inactive and low-value customers  

### 6. Visualization & Insights
Visual charts reveal:

- Spending distribution  
- Frequency patterns  
- Recency heatmaps  
- Segment sizes  
- Segment-wise monetary contribution  

These insights help identify which customer groups should be prioritized.

---

##  Results & Business Value

The RFM model highlights which customer categories drive revenue and which groups need marketing intervention.  
It clearly splits customers into actionable buckets, enabling:

- Better targeting in email campaigns  
- Identifying high-value users for loyalty programs  
- Detecting churn risks early  
- Allocating marketing budgets more efficiently  

---

