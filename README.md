# K-Means Clustering Analysis on Lung Cancer Survey Data Using Snowflake

This project demonstrates how lung cancer survey data stored in a Snowflake
data warehouse can be analyzed using K-Means clustering. The goal is to
group similar survey records and understand hidden patterns in the data
using an unsupervised learning approach.

---

## Project Description

The dataset is retrieved directly from a Snowflake database using the
Snowflake Python connector. After basic preprocessing and label encoding,
K-Means clustering is applied to group the data into clusters. The clustering
quality is evaluated using the silhouette score.

This project focuses on data extraction, preprocessing, and clustering
rather than prediction.

---

## Data Source

- Platform: Snowflake
- Database: CANCER
- Schema: PUBLIC
- Table: SURVEYCANCER

The data is fetched using SQL queries and loaded into a Pandas DataFrame
for analysis.

---

## Tools and Libraries Used

- Python
- Pandas
- Snowflake Connector for Python
- Scikit-learn

---

## Workflow

1. Connect to Snowflake using Python
2. Retrieve survey data using SQL
3. Perform initial data inspection
4. Encode categorical variables using LabelEncoder
5. Apply K-Means clustering
6. Predict cluster labels
7. Evaluate clustering using silhouette score

---

## Clustering Model

- Algorithm: K-Means
- Number of clusters: 2
- Type: Unsupervised Learning
- Evaluation metric: Silhouette Score

---

## Results

The dataset is successfully grouped into two clusters based on survey
attributes. The silhouette score is used to measure how well the data points
fit within their assigned clusters.

---

## How to Run the Project

1. Clone the repository
2. Install required libraries
   ```bash
   pip install pandas scikit-learn snowflake-connector-python
