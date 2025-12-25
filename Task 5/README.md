# 🛍️ Mall Customer Segmentation Analysis

## 📌 Project Overview  
This project applies **machine learning clustering techniques** to segment mall customers based on their demographic and behavioral data. The goal is to identify meaningful customer groups to help businesses design **targeted marketing strategies** and improve customer engagement.

---

## 📊 Dataset Description  
The dataset `Mall_Customers.csv` contains the following features:

- **CustomerID**: Unique identifier  
- **Gender**: Male/Female  
- **Age**: Customer’s age  
- **Annual Income (k$)**: Yearly income in thousands  
- **Spending Score (1-100)**: Mall-assigned spending behavior score  

---

## 🧠 Features  
- **Age_Category**: Binned into Child, Young Adult, Adult, Middle Age, Senior  
- **Income_Category**: Low, Medium, High, Very High Income  
- **Spending_Category**: Low, Moderate, High, Very High Spender  
- **Cluster**: KMeans-assigned segment (5 clusters)  
- **PCA1/PCA2**: Dimensionality-reduced features for visualization  

---

## 🔧 Technical Implementation  

### Libraries Used:
- `pandas`, `numpy`, `matplotlib`, `seaborn`  
- `scikit-learn` (KMeans, StandardScaler, PCA, Pipeline)  

### Steps:
1. **Data Preprocessing** – Removed duplicates, handled missing values, created categorical bins  
2. **Feature Engineering** – Age, Income, Spending categories  
3. **Dimensionality Reduction** – PCA applied to 3 features  
4. **Clustering** – KMeans with 5 clusters  
5. **Visualization** – PCA plots, distribution charts, gender-based analysis  

---

## 📈 Exploratory Data Analysis (EDA)  
- **Age Distribution**: Majority are Young Adults & Adults  
- **Gender Ratio**: Slightly more female customers  
- **Income & Spending**: Most customers have mid-range income and moderate spending scores  
- **Gender-wise Spending**: Females show slightly higher spending across income groups  

---

## 🤖 Model Development  
- Used **KMeans clustering** with `n_clusters=5`  
- Applied **StandardScaler** for normalization  
- Reduced features to **2 principal components (PCA)** for visualization  
- Pipeline: `Scaler → PCA → KMeans`  

### Cluster Insights:
Clusters represent distinct customer profiles such as:
- High income, high spenders  
- Low income, moderate spenders  
- Young adults with average income and spending  

---

## 🏢 Business Impact  
- Enables **personalized marketing** and promotions  
- Helps in **inventory planning** based on customer segments  
- Supports **loyalty program** design for high-value customers  
- Improves **customer retention** through targeted engagement  

---

## 🚀 How to Run  
1. Clone the repository  
2. Install dependencies:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```  
3. Open `Task_5.ipynb` in Jupyter Notebook  
4. Run all cells to reproduce the analysis  

---
