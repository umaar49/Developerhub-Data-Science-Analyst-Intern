# Bank Customer Churn Prediction Analysis

## 📋 Project Overview
This project focuses on predicting bank customer churn using machine learning techniques. By analyzing customer demographics, account information, and transaction patterns, we build models to identify customers likely to leave the bank, enabling proactive retention strategies.

## 🎯 Task Objective
The primary objectives of this project were:
- Predict which customers are likely to churn (leave the bank)
- Identify key factors driving customer churn
- Handle severe class imbalance in the dataset
- Build multiple classification models and select the best performer
- Provide actionable insights for customer retention strategies

## 🛠️ My Approach

### Data Understanding & Initial Analysis
- **Dataset**: 10,000 customer records with 14 features
- **Key Features**: Credit score, geography, gender, age, balance, products, card type
- **Critical Finding**: Severe class imbalance (20% churn rate) requiring specialized handling

### Data Preprocessing & Feature Engineering
- **Missing Values**: Handled missing data points appropriately
- **Feature Encoding**: Converted categorical variables (country,gender,age_group,tenure_group)
- **Feature Scaling**: Applied standardization to numerical features
- **Class Imbalance**: Implemented SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset

### Exploratory Data Analysis
Conducted comprehensive analysis to understand churn patterns:
- **Demographic Analysis**: Age, geography, and gender distributions
- **Financial Analysis**: Balance, credit score, and salary impacts
- **Correlation Analysis**: Identified relationships between features and churn

### Model Development Strategy
Implemented and compared five classification algorithms:
- **Random Forest Classifier**
- **XGBoost Classifier**
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**

## 📊 Results and Insights

### Model Performance Comparison
| Model | ROC-AUC Score | 
|-------|---------------|
| Random Forest | 0.8268 | 
| XGBoost | 0.7993 | 
| SVM | 0.5767 | 
| Logistic Regression | 0.5687 | 
| KNN | 0.5189 | 

### Key Churn Drivers Identified

#### 🔍 Top Factors Influencing Customer Churn:
1. **Age group young**
2. **Active member**
3. **Products number**
4. **Country france**
5. **Gender male**


#### 💼 Business Impact:
- **Proactive Retention**: Identify at-risk customers before they leave
- **Targeted Marketing**: Develop personalized retention offers
- **Product Strategy**: Encourage multi-product relationships to reduce churn
- **Resource Optimization**: Focus retention efforts on high-probability segments

### Technical Achievements

#### 🎯 Model Performance:
- **Random Forest** achieved 82% ROC-AUC score
- **Effective Imbalance Handling**: SMOTE significantly improved minority class prediction
- **Feature Importance**: Clear identification of key churn predictors
- **Model Robustness**: Consistent performance across different customer segments

#### 📊 Validation Strategy:
- Comprehensive train-test split validation
- ROC-AUC as primary metric for imbalanced classification
- Feature importance analysis for model interpretability
- Multiple model comparison for optimal selection

## 💡 Conclusion

The Bank Customer Churn Prediction project successfully demonstrates the power of machine learning in customer retention strategies. By achieving 82% predictive accuracy with Random Forest, the model provides banks with a powerful tool to:

- **Reduce Customer Acquisition Costs** by focusing on retention
- **Improve Customer Satisfaction** through proactive engagement
- **Optimize Marketing Resources** by targeting high-risk segments
- **Enhance Product Development** based on churn driver insights

**The key takeaway**: Customer churn is highly predictable when analyzing the right combination of demographic, financial, and behavioral data. Banks that leverage these insights can significantly improve customer retention and overall business performance.

This project showcases how data science can transform customer relationship management in the banking sector, turning reactive problem-solving into proactive strategic advantage.
