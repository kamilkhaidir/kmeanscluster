# 🛍️ Mall Customer Segmentation with K-Means

This project performs **customer segmentation** using the **K-Means clustering algorithm** on the **Mall Customers dataset**. The goal is to group customers based on their annual income and spending behavior to help businesses target marketing strategies more effectively.

---

## 📁 Dataset

- **Source**: [Mall Customers Dataset on Kaggle](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial)
- **Features used**:
  - `Annual Income (k$)`
  - `Spending Score (1-100)`
  - *(Optional)* `Age`

---

## 🔧 Methodology

1. **Data Preparation**
   - Imported and previewed dataset using pandas
   - Selected relevant numerical features
   - Scaled the data using `StandardScaler` to normalize feature values

2. **Optimal Cluster Selection**
   - Applied the **Elbow Method** to determine the ideal number of clusters (k)
   - Plotted inertia vs. number of clusters

3. **Clustering**
   - Used `KMeans` from `sklearn.cluster` with `k = 3`
   - Assigned cluster labels back to the original DataFrame
   - Analyzed each cluster using group-wise averages

4. **Visualization**
   - Plotted clusters using `seaborn.scatterplot`
   - Interpreted clusters based on average income and spending

---

## 📊 Results & Interpretation

| Cluster | Average Income | Average Spending | Interpretation                     |
|---------|----------------|------------------|-------------------------------------|
| 0       | 44.15k         | 49.83            | Mid-income, average spenders        |
| 1       | 86.54k         | 82.13            | High-income, high spenders (VIPs)   |
| 2       | 87.00k         | 18.63            | High-income, low spenders (cautious)|

---

## 📌 Key Takeaways

- K-Means is effective for customer segmentation when data is numeric and clean.
- Spending patterns don’t always correlate with income.
- Cluster analysis can provide actionable insights for marketing strategies.

---

## 💻 Technologies Used

- Python (Jupyter Notebook)
- pandas, matplotlib, seaborn, scikit-learn

---

## 📎 How to Use

1. Clone the repo or download the `.ipynb` file
2. Open in Jupyter Notebook or Google Colab
3. Run the notebook to reproduce results
4. Optional: Replace the dataset with your own customer data to test further

---

