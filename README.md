
# Customer Segmentation and Revenue Prediction

## Project Overview

Full codes and analysis can be viewed here: [Cusomter Segmentation Revenue Prediction for Online Retail](https://github.com/an-pk-chu/Customer-Segmentation-Revenue-Prediction-for-Online-Retail/blob/main/Customer_Segmentation_and_Prediction_Project.ipynb)

This project involves analyzing customer data from an online retail store to derive insights and develop actionable business strategies. The analysis focuses on two main objectives:

1. **Customer Segmentation**:
   - Use clustering techniques to group customers based on their purchasing behaviors.
   - Identify actionable strategies for each customer segment to improve engagement and revenue.

2. **Revenue Prediction**:
   - Build a regression model to predict revenue using key features.
   - Analyze the impact of different features on revenue and provide business recommendations.

---

## Data Description

The dataset used in this analysis contains information on online retail transactions. The primary features include:
- **InvoiceNo**: Unique identifier for each transaction.
- **StockCode**: Item code for the products purchased.
- **Description**: Product description.
- **Quantity**: Number of items purchased.
- **InvoiceDate**: Date of the transaction.
- **UnitPrice**: Price per unit.
- **CustomerID**: Unique identifier for each customer.
- **Country**: Country of the customer.

---

## Key Features

### **Customer Segmentation Features**
1. **Revenue**: Total spending by a customer.
2. **Quantity**: Total number of items purchased by a customer.
3. **Number of Orders**: Total number of unique transactions by a customer.
4. **Recency**: Days since the customer's last purchase.

### **Revenue Prediction Features**
1. **Quantity**: Number of items purchased in a transaction.
2. **UnitPrice**: Price per unit of the product.
3. **OrderSize**: Revenue per item (Revenue / Quantity).

---

## Tools and Libraries

The following tools and libraries were used in the project:
- **Python Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Visualization Tools**: Matplotlib, Seaborn
- **Clustering Algorithm**: K-Means
- **Regression Model**: Linear Regression

---

## Steps in Analysis

### **1. Data Preparation**
- Filtered dataset to include only transactions from the United Kingdom.
- Handled missing values and duplicates.
- Added new features: `Revenue` and `OrderSize`.

### **2. Customer Segmentation**
- Selected features: `Revenue`, `Quantity`, `NumberOfOrders`, `Recency`.
- Standardized features using `StandardScaler`.
- Applied K-Means clustering to group customers into four segments.
- Visualized clusters using PCA for dimensionality reduction.

### **3. Revenue Prediction**
- Defined `Revenue` as the target variable.
- Built a linear regression model using `Quantity`, `UnitPrice`, and `OrderSize` as features.
- Evaluated model performance using R², MAE, and RMSE.
- Identified `Quantity` as the feature with the strongest impact on revenue.

---

## Results

### **Customer Segmentation**
- Identified four customer segments:
  - **Low-value, infrequent customers**: Re-engage through promotions.
  - **Moderate-value, medium-engagement customers**: Incentivize with loyalty programs.
  - **High-value, high-engagement customers**: Retain through VIP benefits.
  - **Ultra high-value bulk buyers**: Maintain loyalty with personalized offers and account managers.

### **Revenue Prediction**
- Linear regression model achieved an R² score of 0.72.
- Key finding: Quantity (+1.02) as the strongest revenue driver and unit price (–0.05) as slightly negative; advised management to prioritize sales volume strategies (bundling, upselling, discounts) over price increases to maximize long-term growth.

## Visualizations
1. **Cluster Visualization**: PCA plot showing customer segments.
2. **Predicted vs. Actual Revenue**: Scatter plot to evaluate regression performance.
3. **Cluster Characteristics**: Bar plots of average revenue, quantity, number of orders, and recency for each cluster.

---

## Business Recommendations

### **Customer Segmentation Strategies**
- **Cluster 0**: Implement re-engagement campaigns.
- **Cluster 1**: Offer loyalty rewards to increase purchase frequency.
- **Cluster 2**: Retain high-value customers with exclusive programs.
- **Cluster 3**: Provide dedicated account management and volume discounts.

### **Revenue Growth Strategies**
- Focus on increasing `Quantity` through bundle offers and volume discounts.
- Address outliers by analyzing large transactions or return behaviors.

---

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   ```
2. **Install Dependencies**:
   Ensure Python and required libraries are installed. Use the following command to install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Analysis**:
   Open the Python script or Jupyter Notebook and execute the cells sequentially.

---

## Future Improvements

- Use non-linear models (e.g., Random Forest or Gradient Boosting) for better revenue predictions.
- Incorporate additional features like customer loyalty, seasonality, and promotional campaigns.
- Apply advanced clustering techniques (e.g., DBSCAN or Hierarchical Clustering) for deeper segmentation insights.

---

## Contact

For any questions or suggestions, feel free to reach out:
  
**Email**: chuphankhanhan@gmail.com  
**GitHub**: (https://github.com/an-pk-chu)
