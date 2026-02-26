# PREDICTIVE ANALYSIS USING MACHINE LEARNING

## 📌 Project Overview
This project demonstrates **predictive analysis** using machine learning on an **Online Retail Dataset**.  
The objective is to analyze customer behavior, perform feature engineering, and build a model to **predict high-value customers** based on transactional data.


## 🎯 Objective
- Perform data cleaning and exploratory analysis on a retail dataset  
- Engineer features to quantify customer behavior (**RFM: Recency, Frequency, Monetary**)  
- Build a machine learning model to predict high-value customers  
- Evaluate model performance using metrics such as accuracy and feature importance  
- Generate actionable business insights from predictive modeling  



## 🗂 Dataset Information
- **Dataset Name:** Online Retail Dataset  
- **Source:** UCI Machine Learning Repository  
- **Format:** CSV  
- **Records:** ~541,909 transactions  

The dataset contains online retail transactions including:  
- Invoice details  
- Product codes and descriptions  
- Quantity and price  
- Customer IDs  
- Transaction date  
- Country  



## 🛠 Tools & Technologies Used
- Python  
- Pandas & NumPy  
- Plotly & Matplotlib  
- Scikit-learn (Machine Learning)  
- Jupyter Notebook / Google Colab  



## ⚙️ Project Workflow

### Step 1: Environment Setup
- Installed required libraries (`plotly`, `scikit-learn`)  
- Imported Python packages for data processing, visualization, and machine learning  

### Step 2: Data Loading
- Loaded CSV dataset into a Pandas DataFrame  
- Displayed dataset shape and previewed first few rows  

### Step 3: Data Cleaning
- Removed rows with missing `CustomerID`  
- Removed returns and transactions with non-positive `Quantity` or `UnitPrice`  
- Checked for duplicates and reset index  

### Step 4: Feature Engineering
- Created **Revenue column**: `Revenue = Quantity × UnitPrice`  
- Converted `InvoiceDate` to datetime format  
- Built **RFM table** per customer:
  - **Recency:** Days since last purchase  
  - **Frequency:** Number of transactions  
  - **Monetary:** Total spending  

### Step 5: Exploratory Data Analysis (EDA)
- Analyzed distribution of customer spending  
- Visualized Recency vs Monetary value  
- Analyzed country-wise revenue contribution  

### Step 6: Machine Learning Modeling
- Labeled customers as **High-Value (1)** or **Low-Value (0)** based on median Monetary value  
- Scaled features using `StandardScaler`  
- Split dataset into training and testing sets  
- Trained **Random Forest Classifier** to predict high-value customers  

### Step 7: Model Evaluation
- Evaluated model using:
  - Accuracy score  
  - Classification report (Precision, Recall, F1-Score)  
  - Confusion matrix  
- Determined feature importance to understand drivers of high customer value  

### Step 8: Data Visualization
- Visualized results using:
  - Plotly tables for sample data  
  - Scatter plots for Recency vs Monetary  
  - Bar charts for country revenue  
  - Confusion matrix and feature importance  


## 📊 Key Insights
- **High-value customers** typically have higher frequency of purchases and greater total spending  
- Revenue distribution is skewed: a small percentage of customers contribute disproportionately to total revenue  
- European countries generated the majority of revenue  
- Feature importance showed that **Frequency** and **Monetary** are the most predictive features for customer value  


## ✅ Conclusion
This project demonstrates how **machine learning can be applied to retail data** to predict high-value customers.  

**Key Takeaways:**  
- RFM analysis is effective for feature engineering in customer segmentation  
- Random Forest provides both accurate predictions and interpretable feature importance  
- Predictive modeling can guide targeted marketing and customer retention strategies  
