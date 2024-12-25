# Term-2_Project-1
Project Report
Title: Build Unsupervised Learning Models using Python: Clustering {Hierarchical | K-Means}
Prepared By:
055029: Prachi Lakra
055060: Chirag Singla
Group Number-20
Term-2
Project-Project 1
1. Project Information
This project centers on the examination of a dataset related to import-export transactions. The aim is to discover trends, detect anomalies, and extract actionable insights that can support enhanced decision-making processes.

# Approach
The project employs a blend of statistical and machine learning methodologies to analyze the data and derive significant insights. The ultimate goal is to propose recommendations for enhancing trade efficiency and pinpointing key market segments or anomalies that may impact business strategies.

2. Description of Data
The structure of the data includes multiple columns related to import-export transactions.

Subjective Description of the Data
The dataset under analysis comprises 16 columns and 15,000 rows, representing transactional records in the domain of import-export activities. Below is a subjective interpretation of the dataset's attributes:

Transaction_ID:

A unique identifier for each transaction, essential for tracking and referencing specific records.
Country:

Specifies the country involved in the transaction, offering insights into geographic distribution and facilitating the analysis of trade patterns across regions.
Product:

Provides details about the goods involved in the trade, enabling the identification of high-demand or high-value products.
Import_Export:

Indicates whether the transaction is an import or export, facilitating the study of trade flow directions.
Quantity:

Reflects the volume of goods traded in unit quantities, aiding in the assessment of transaction scale.
Value:

Represents the monetary value of the transaction, crucial for evaluating trade impact and market size.
Date:

The transaction date, which supports time-series analysis to uncover trends, seasonality, and anomalies in trade activities.
Category:

A broad classification of the product, enabling aggregated insights through segmentation.
Port:

Indicates the port of entry or exit, critical for understanding logistics and transportation patterns.
Customs_Code:

A numerical classification assigned by customs, supporting regulatory compliance analysis.
Weight:

Denotes the weight of traded goods, often in kilograms or tons, complementing the Quantity column for logistics planning.
Shipping_Method:

Describes the mode of transport (e.g., air, sea, or land), pivotal for analyzing cost-efficiency and transit times.
Supplier:

Identifies the provider of goods, aiding in the evaluation of supply chains and vendor management.
Customer:

Specifies the recipient or buyer of goods, offering insights into demand-side dynamics and customer segmentation.
Invoice_Number:

A unique identifier for billing and payment, ensuring traceability and financial accountability.
Payment_Terms:

Describes the terms of payment, aiding in the analysis of financial arrangements and credit practices.
3. Project Objectives | Problem Statements
Identify Product Clusters

Use unsupervised learning techniques to group product categories that are frequently exported or imported together, uncovering relationships and co-occurrence patterns in trade data.
Discover Market Segmentation

Analyze trade patterns to identify markets with similar buying or selling behaviors, enabling targeted marketing and resource allocation strategies.
Detect Anomalies in Transactions

Identify unusual trends, such as price fluctuations, abnormally high or low quantities, or irregular trade routes, which could indicate potential errors, fraud, or unique opportunities.
Optimize Trade Routes and Shipping Methods

Evaluate patterns in port usage and shipping methods to optimize logistics, reduce costs, and improve delivery times.
Uncover Seasonal Trends

Analyze time-series data to detect seasonal variations or recurring patterns in trade volumes for better demand forecasting and inventory management.
Spot High-Value Product Groups

Cluster products and categories to identify high-value goods that drive trade revenues, aiding in prioritization and strategic focus.
Explore Supplier-Customer Relationships

Investigate transactional data to detect consistent partnerships or dependencies between suppliers and customers for improved supply chain management.
Evaluate Payment Practices

Analyze patterns in payment terms and invoice values to identify common practices, delayed payments, or potential risks in financial transactions.
4. Analysis of Data:
The dataset underwent preprocessing, normalization, and clustering through K-Means, Hierarchical Clustering, and Agglomerative Clustering techniques. Silhouette scores were computed to determine the optimal number of clusters. Visualization tools like the elbow plot and dendrogram helped identify cluster boundaries and relationships.
5 Observations & Findings
Based on the provided dendrogram and silhouette score plots:

Observations
Hierarchical Clustering (Dendrogram):
Clear hierarchical structures are evident, with significant vertical gaps suggesting potential cluster divisions.
A threshold can be set to determine the optimal number of clusters.
Silhouette Scores:
The silhouette scores decrease as the number of clusters increases, indicating a diminishing cluster compactness and separation.
A high silhouette score for 2 clusters suggests that the dataset is well-separated into two distinct groups.
Adding more clusters reduces the score, which might imply over-segmentation or less meaningful divisions.
Findings
Optimal Clustering:

Two clusters strike a balance between separation and compactness. However, additional clusters provide finer segmentation based on specific needs.
Cluster Characteristics:

Identified clusters represent groups of similar data points, such as product categories or market segments.
Trade-off Between Simplicity and Detail:

While simpler segmentation (e.g., two clusters) is interpretable, higher granularity (e.g., 3–5 clusters) may better suit targeted use cases.
6 Manegerial Insights
Managerial Insights
Presence of Two Distinct Groups:

The silhouette score analysis reveals that the dataset can be optimally divided into two distinct groups or clusters. This indicates that the data points within each group share significant similarities, while the groups themselves are well-separated.
Strategic Implications of the Two Groups:

These two groups may represent key segments such as:
Product Categories: Two broad product types dominating import/export transactions.
Market Segments: Distinct buyer or supplier groups with varying trade behaviors.
Geographical Trends: Regions with different trade volumes or patterns.
Simplified Segmentation:

Keeping two clusters allows for a high-level segmentation, making it easier to develop targeted strategies without overcomplicating the analysis.
Actionable Strategies:

Focus on tailored marketing strategies for each group to maximize trade efficiency.
Design customized supply chain processes for each group to optimize resource allocation and logistics.
Investigate outliers within each group to identify unique opportunities or potential risks.
Validation of Cluster Use:

Before finalizing strategies, validate the group composition with domain knowledge to ensure the clustering reflects meaningful trade characteristics.
Further Insights with Supervised Learning:

Implementing supervised learning can refine these clusters by predicting specific outcomes, such as trade volume, revenue, or anomaly detection, enabling precise strategies for targeted business optimization.
