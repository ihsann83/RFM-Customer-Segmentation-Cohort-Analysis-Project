# RFM-Customer-Segmentation-Cohort-Analysis-Project

This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

First of all, I used exploratory data analysis and data visualization techniques in order to observe the structure of the data and missing values.
 
I did descriptive analysis to understand the relationship of the features to each other and clear the noise and missing values in the data. Then, the data set became ready for RFM analysis.

Before starting the RFM Analysis, I did some analysis regarding the distribution of "Orders", "Customers" and "Countries". The company could develop its sales policies and contribute to the correct use of resources with those analyzes.

I noticed that the UK not only has the most sales revenue, but also the most customers. So I continued to analyze only UK transactions in the next RFM Analysis, Customer Segmentation and K-Means Clustering topics.

Then, I began RFM Analysis which is a customer segmentation technique based on customers' past purchasing behavior.

By using RFM Analysis, you can enable companies to develop different approaches to different customer segments so that they can get to know their customers better, observe trends better, and increase customer retention and sales revenues.

I calculated the Recency, Frequency and Monetary values of the customers in the RFM Analysis with UK transactions. Ultimately, I created an RFM table containing these values.

In the Customer Segmentation section, I created an RFM Segmentation Table where the customers were segmented by using the RFM table. For example, I labeled the best customer as "Big Spenders" and the lost customer as "Lost Customer".

I segmented the customers based on their recency, frequency, and monetary values. In addition to this, I used the K-Means algorithm to segment the customers. Then I compared the results.

Before applying K-Means Clustering, I did data pre-processing to examine feature correlations and distributions. In addition to this, the data should be normalized which I applied K-Means.

On the other hand, I informed the K-means algorithm about the number of clusters it will predict. I tried the * Elbow method * and * Silhouette Analysis * to find the optimum number of clusters.

After the above operations, I made cluster estimation with K-Means. I visualized the cluster distribution by using a scatter plot. I observed the properties of the resulting clusters with the help of the boxplot. Thus I was able to tag clusters and interpret results.

Finally, I did Cohort Analysis with the data I used at the beginning, regardless of the analysis I have done before. Cohort analysis is a subset of behavioral analytics that takes the user data and breaks them into related groups for analysis. This analysis can further be used to do customer segmentation and track metrics like retention, churn, and lifetime value.

# Tasks

#### 1. Data Cleaning & Exploratory Data Analysis

- Import Modules, Load Data & Data Review
- Follow the Steps Below

    *i. Take a look at relationships between InvoiceNo, Quantity and UnitPrice columns.*
    
    *ii. What does the letter "C" in the invoiceno column mean?*
    
    *iii. Handling Missing Values*
    
    *iv. Clean the Data from the Noise and Missing Values*
    
    *v. Explore the Orders*
    
    *vi. Explore Customers by Country*
    
    *vii. Explore the UK Market*
    
#### 2. RFM Analysis

- Follow the steps below

   *i. Import Libraries*
   
   *ii. Review "df_uk" DataFrame (the df_uk what you create at the end of the Task 1)*
   
   *iii. Calculate Recency*
   
   *iv. Calculate Frequency*
   
   *v. Calculate Monetary Values*
   
   *vi. Create RFM Table*

#### 3. Customer Segmentation with RFM Scores
- Calculate RFM Scoring

    *i. Creating the RFM Segmentation Table*
 
- Plot RFM Segments

#### 4. Applying K-Means Clustering
- Data Pre-Processing and Exploring

    *i. Define and Plot Feature Correlations*
 
    *ii. Visualize Feature Distributions*
 
    *iii. Data Normalization*

- K-Means Implementation

    *i. Define Optimal Cluster Number (K) by using "Elbow Method" and "Silhouette Analysis"*
 
    *ii. Visualize the Clusters*
 
    *iii. Assign the label*
 
    *iv. Conclusion*
 
#### 5. Create Cohort and Conduct Cohort Analysis
- Future Engineering

    *i. Extract the Month of the Purchase*
 
    *ii. Calculating time offset in Months i.e. Cohort Index*
 
- Create 1st Cohort: User Number & Retention Rate 

    *i. Pivot Cohort and Cohort Retention*
 
    *ii. Visualize analysis of cohort 1 using seaborn and matplotlib*

- Create 2nd Cohort: Average Quantity Sold 

    *i. Pivot Cohort and Cohort Retention*
 
    *ii. Visualize analysis of cohort 2 using seaborn and matplotlib*

- Create 3rd Cohort: Average Sales

    *i. Pivot Cohort and Cohort Retention*
 
    *ii. Visualize analysis of cohort 3 using seaborn and matplotlib*
    
# Determines

Using the [Online Retail dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail) from the UCI Machine Learning Repository for exploratory data analysis, ***Customer Segmentation***, ***RFM Analysis***, ***K-Means Clustering*** and ***Cohort Analysis***.

This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

Feature Information:

**InvoiceNo**: Invoice number. *Nominal*, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation. 
<br>
**StockCode**: Product (item) code. *Nominal*, a 5-digit integral number uniquely assigned to each distinct product.
<br>
**Description**: Product (item) name. *Nominal*. 
<br>
**Quantity**: The quantities of each product (item) per transaction. *Numeric*.
<br>
**InvoiceDate**: Invoice Date and time. *Numeric*, the day and time when each transaction was generated.
<br>
**UnitPrice**: Unit price. *Numeric*, Product price per unit in sterling.
<br>
**CustomerID**: Customer number. *Nominal*, a 5-digit integral number uniquely assigned to each customer.
<br>
**Country**: Country name. *Nominal*, the name of the country where each customer resides.

    
