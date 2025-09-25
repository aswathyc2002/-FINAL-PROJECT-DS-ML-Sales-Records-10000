# -FINAL-PROJECT-DS-ML-Sales-Records-10000


Final Project Report: Sales Data Analysis 


📝 Project Title: Exploratory Data Analysis and Predictive Modeling on Global Sales Records

1. 📁 Dataset Overview


The dataset contains 10,000 sales records across various regions, countries, and item types. It includes details such as order dates, sales channels, units sold, pricing, revenue, costs, and profits.

Dataset Dimensions:

Rows: 10,000 Columns: 14

📌 Column Descriptions:

.Column - Description--- .Region - Sales region, .Country - Country where the sale occurred, .Item Type - Type of item sold, .Sales Channel - Online or Offline sales, .Order Priority- Priority level (L, M, H, C), .Order Date - Date when order was placed , .Order ID - Unique order identifier, .Ship Date - Date when order was shipped, .Units Sold - Number of units sold , .Unit Price - Selling price per unit, .Unit Cost - Cost per unit .Total Revenue - Total revenue = Units Sold × Unit Price, .Total Cost - Total cost = Units Sold × Unit Cost, .Total Profit - Total profit = Total Revenue - Total Cost,

2. 🔍 Data Preprocessing


Converted Order Date and Ship Date to datetime format Checked for missing values Filtered only numeric columns for machine learning models Encoded target variables where needed (e.g., using LabelEncoder for classification)

3. 📈 Exploratory Data Analysis (EDA)


Top Selling Regions: Identified which regions generated the most revenue Sales Channel Analysis: Compared online vs offline performance Item Type Trends: Found most and least profitable item types Scatter Plot: Total Cost vs Total Profit to explore linearity Correlation Heatmap: Identified relationships between numeric variables

4. 🧠 Predictive Modeling


Supervised Learning (Classification): Target Variable: Unit Price (encoded into classes) Features: All other numeric features

Models used:

Logistic Regression
Decision Tree
Random Forest
K-Nearest Neighbors
Gradient Boosting
✅ Accuracy Comparison: Model Accuracy Decision Tree 1.000 Random Forest 1.000 Gradient Boosting 1.000 Logistic Regression 0.9728 K-Nearest Neighbors 0.5899

5.🔍 Best Model:


Random Forest and Gradient Boosting performed best with 100% accuracy, suggesting very high predictive power — though overfitting needs to be ruled out with cross-validation.

6. 📊 Unsupervised Learning (Clustering)


Used K-Means Clustering with Elbow Method to find optimal number of clusters Applied PCA for 2D visualization of clusters Found distinct groups based on cost and profit features

7. 🎯 Key Insights


Sales vary significantly by region and item type Profit is directly influenced by unit cost and price Ensemble models outperform others in classification tasks KNN underperformed — not suitable for this dataset without tuning

8. 📌 Recommendations


Use ensemble models like Random Forest for profit prediction Segment marketing by region and item type for maximum profit Consider revisiting underperforming products or regions

9. 📁 Future Improvements


Add temporal analysis (monthly trends) Use cross-validation for better generalization Incorporate external features like promotions or seasonal data

10. ✅ Final Conclusion


This project successfully analyzed and modeled a large sales dataset, offering valuable insights into sales performance and profitability across different regions and item types. Ensemble models such as Random Forest and Gradient Boosting delivered outstanding performance, achieving perfect classification accuracy. However, such results should be interpreted with caution due to potential overfitting and the absence of cross-validation.


Exploratory Data Analysis (EDA) revealed strong linear relationships between total cost, revenue, and profit, and clustering techniques helped identify patterns within sales data using unsupervised learning.


Overall, the project demonstrates the power of machine learning for predictive sales analysis and decision support. However, for a more robust and production-ready solution, further steps like model tuning, validation, and business integration are recommended.


--End--
