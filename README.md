# Customer-Segmentation-for-E-Commerce
Capstone Project - Customer Segmentation for E-commerce
### Project Title
Capstone Project - Customer Segmentation for E-commerce
**Rahul Tantak**

#### Executive summary
In today’s fast-moving e-commerce world, many businesses still use the same marketing approach for all customers. This often leads to poor engagement and low sales because it doesn’t reflect how different people shop. To fix this, goal is to use a customer shopping dataset, which includes useful details like age, gender, location, how much people spend, how often they shop, what they buy, what category of items, sizes etc, and how they pay. The goal is to build a smart system that groups customers based on their shopping habits. These groups will help businesses send more personalized offers that match each customer’s style and needs. 

#### Rationale
Why should anyone care about this question?
By creating clear customer segments, the marketing team can stop using generic messages and start sending personalized offers that match each group’s habits. This approach is expected to boost repeat purchases and increase overall sales by at least 10%.

#### Research Question
What are you trying to answer?
The main goal of this project is to build a machine learning model that groups customers based on how they shop, how often they buy, how much they spend, and how recently they made a purchase (known as RFM: Recency, Frequency, Monetary).

#### Data Sources
What data will you use to answer you question?
This project will use the "Customer Shopping Trends" dataset. This dataset is sourced from Kaggle and contains 3,900 records with 18 columns capturing both demographic and behavioral attributes of shoppers. It includes fields such as age, gender, location, item purchased, purchase amount, frequency of purchases, payment method, and subscription status, making it suitable for customer segmentation and trend analysis.
Source Platform: Kaggle
Dataset Name :   Customer Shopping Trends Dataset.
Dataset Link : https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset

#### Methodology
What methods are you using to answer the question?
The project will follow a structured data science lifecycle:

1. Data Acquisition: Fetch the dataset from Kaggle using its API.
2. Preprocessing: Clean the data by handling missing values, removing canceled transactions, and ensuring correct data types.
3. EDA: Analyze the data to understand distributions and relationships between features like quantity, price, and customer purchase patterns.
4. Feature Engineering: Create the core RFM (Recency, Frequency, Monetary) features for each customer, along with other metrics like average basket size and product diversity.
5. Modeling: Train clustering models (e.g., K-Means Clustering, Hierarchical Clustering) to group customers into meaningful segments for the business to run targeted marketing campaigns / offers.
6. Evaluation & Interpretation: Assess the quality of clusters using metrics like the Silhouette Score and, most importantly, by analyzing the characteristics of each segment to create meaningful personas.
7. Final Expected Results - Reporting & Visualization: Create a dashboard in Excel or Power BI to present the customer segments, their profiles, and also a list of actionable marketing recommendations to stakeholders.

#### Results
What did your research find?

1. Kmeans and Hierarchical clustering models were implemeted.
2. 7 key features which have a high corelation were selected as seen from the correlation HeatMap.
3. For KMeans clustering an optimal K of 3 was chosen based on the elblow curve.
4. Similarly, for Hierarchical Clustering an optimal K of 3 was chosen as observed from the Dendrogram hierarchy. (The dendogram suggested 4 clusters, out of which 3 were distinct and 4th was a very small cluster which was ignored).
5. Silhouette scores and Davies-Bouldin Index of both method were evaluated.
6. It was observed that the we can clearly identify 3 disctinct clusters (segmants).
7. The new customer data added formed a distinct new cluster with a very low intra cluster distance and high intercluster distance. The intra-clsuter distance was observed to be compatarively low as expected. Inter-cluster distance was not that high for two clusters
8. Silhouette scores were found to be in mid-range though not very close to 1
9. Davies-Bouldin index was found to be relatively high and not close to 0.
10. The clustering via KMeans method showed more clear disctnction / boundaris of the clusters for the same set of features. This was also supprted by better values for the metrics - Silhouette scores and Davies-Bouldin Index.
11. This project successfully executed a comprehensive data science workflow, encompassing extensive Exploratory Data Analysis (EDA), data cleaning, and robust feature engineering on customer shopping trend data.
12. Key achievements include the successful identification and handling of data quality issues, the creation of insightful new features like 'Purchase Recency' and 'Avg Spend Per Purchase', and the effective application of clustering techniques.
13. Successfully segmented customers into 3 distinct groups using both K-Means and Hierarchical clustering. K-Means emerged as the preferred model, demonstrating clearer cluster boundaries and better performance based on Silhouette scores and Davies-Bouldin Index.


#### Next steps
What suggestions do you have for next steps?

1. Deep Dive into Customer Segments: Conduct an in-depth analysis of each identified customer cluster to understand their unique demographics, purchasing behaviors, and preferences. This will inform personalized business strategies.
2. Develop Targeted Strategies: Based on segment insights, formulate and implement targeted marketing campaigns, product recommendations, and loyalty programs designed to maximize engagement and value for each specific customer group.
3. Model Refinement and Exploration: Experiment with different feature sets, and continuously monitor cluster stability and evolution over time to ensure model relevance.
4. Predictive Analytics: Leverage the established customer segments as a foundation for advanced predictive modeling, such as forecasting future purchase behavior, predicting churn risk, or estimating Customer Lifetime Value (CLTV).

#### Outline of project
Capstone Project -  UC Berkley - PG Program in AI and Machine Learning.ipynb

##### Contact and Further Information
Rahul Tantak (rahul.tantak@gmail.com)
