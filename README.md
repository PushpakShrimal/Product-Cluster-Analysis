# Product-Cluster-Analysis
🛍️ Customer segmentation using K-Means clustering to identify target groups from purchase data. Features Elbow Method for cluster optimization and marketing strategy suggestions.


# 🛍️ Customer Segmentation using K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.0%2B-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5%2B-blue?logo=matplotlib)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 🎯 Project Goal

The goal of this project is to perform a customer segmentation analysis to identify distinct groups within a customer base. By using **K-Means Clustering**, an unsupervised machine learning algorithm, we can uncover patterns in customer behavior based on their annual income and spending score. The resulting segments provide actionable insights for creating targeted and effective marketing strategies.

## 📊 The Dataset

The analysis is performed on a customer dataset (`dataset.csv`) which contains the following key features for clustering:
-   `Annual Income (k$)`: The annual income of the customer.
-   `Spending Score (1-100)`: A score assigned to the customer based on their spending behavior.

## 🛠️ Methodology

The project follows a systematic approach to uncover customer segments:

1.  **Data Preprocessing:** The dataset was loaded, and the relevant features (`Annual Income` and `Spending Score`) were selected for the clustering task.
2.  **Finding the Optimal Number of Clusters:** The **Elbow Method** was used to determine the optimal number of clusters (k) for the K-Means algorithm. By plotting the Within-Cluster Sum of Squares (WCSS) for various values of k, the "elbow" point was identified at **k=5**, indicating the most effective number of segments.

    *(You can add a screenshot of your Elbow Method plot here)*

3.  **K-Means Model Training:** A K-Means model was trained on the data with `k=5` to group the customers into five distinct clusters.
4.  **Cluster Visualization:** The final customer segments were visualized using a scatter plot to clearly show the distinct groups based on their income and spending score.

## 💡 Customer Segments Identified

The K-Means algorithm successfully identified five distinct customer segments, each with unique characteristics:

*(You should add a screenshot of your final cluster visualization plot here)*

-   **Cluster 1: Careful Spenders** (High Income, Low Spending Score)
    -   These customers earn a high income but are cautious with their spending.
-   **Cluster 2: Standard Customers** (Average Income, Average Spending Score)
    -   This group represents the average customer with balanced income and spending habits.
-   **Cluster 3: Target Group (Ideal Customers)** (High Income, High Spending Score)
    -   These are the most valuable customers, with high income and a high propensity to spend.
-   **Cluster 4: High Spenders** (Low Income, High Spending Score)
    -   These customers spend a lot despite having a lower income, possibly on credit or specific interests.
-   **Cluster 5: Low Spenders** (Low Income, Low Spending Score)
    -   This segment consists of customers with low income who also spend very little.

## 📈 Business Impact & Marketing Strategy

This segmentation allows for tailored marketing strategies to maximize engagement and profitability for each group:

| Cluster Name         | Characteristics                    | Recommended Marketing Strategy                                           |
| -------------------- | ---------------------------------- | ------------------------------------------------------------------------ |
| **Target Group** | High Income, High Spending         | Engage with loyalty programs, exclusive previews, and premium product offers. |
| **Careful Spenders** | High Income, Low Spending          | Target with high-quality product promotions and investment-worthy offers.      |
| **Standard Customers**| Average Income, Average Spending   | Provide standard offers, seasonal promotions, and build brand loyalty.     |
| **High Spenders** | Low Income, High Spending          | Offer discounts, EMI options, and promotions on trendy or aspirational items. |
| **Low Spenders** | Low Income, Low Spending           | Market essential products, budget-friendly deals, and value packs.       |

## 🚀 How to Run this Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/PushpakShrimal/Customer-Segmentation-KMeans.git](https://github.com/PushpakShrimal/Customer-Segmentation-KMeans.git)
    cd Customer-Segmentation-KMeans
    ```
2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate
    ```
3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook notebooks/Project_6_(Product_Cluster_Analysis).ipynb
    ```

---
