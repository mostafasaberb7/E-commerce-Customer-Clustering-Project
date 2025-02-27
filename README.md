# E-commerce-Customer-Clustering-Project

## Project Overview
This project focuses on customer segmentation for an e-commerce platform using unsupervised learning techniques. The goal is to group customers based on their transaction behavior and demographic information to provide insights for marketing and promotional strategies.

## Data
The dataset consists of four main sources:
- **Customers**: Information about customers, including demographics.
- **Genders**: Gender details for each customer.
- **Cities**: City information for each customer.
- **Transactions**: Transactional data of customers with details like coupon usage and transaction status.

The datasets are merged to form a unified dataframe containing the customer demographic data and their transaction behavior.

## Model Approach
We used KMeans clustering to segment customers into distinct groups based on features such as:
- Gender
- City
- Transaction status
- Coupon usage frequency

### Preprocessing:
- **Label Encoding**: Categorical features (gender, city, transaction status) were label-encoded to prepare for clustering.
- **Feature Scaling**: Numerical features like coupon usage frequency were scaled using `StandardScaler` to ensure uniformity in feature values.

### Clustering:
- We applied **KMeans** clustering and evaluated the optimal number of clusters using the **Elbow Method** and the **Silhouette Score** to find the best segmentation.

## Evaluation Metrics
- **Inertia**: Measures the sum of squared distances of samples to their closest cluster center.
- **Silhouette Score**: A higher score indicates that the clusters are well-separated and dense.
- **Elbow Method**: Used to determine the optimal number of clusters by plotting inertia against the number of clusters.

## Key Findings
- The KMeans model segmented the customers into three distinct clusters.
- Using the Elbow Method, we identified that three clusters provided a good balance between performance and interpretability.
- The clusters are characterized by distinct patterns in coupon usage frequency, transaction status, and demographics, providing actionable insights for targeted marketing.

## Conclusion
This project demonstrates how unsupervised learning techniques can be applied to e-commerce customer data to reveal meaningful customer segments. The insights from clustering can help the business better target promotions and personalize customer experiences.
"""

