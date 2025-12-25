# Bank Term Deposit Subscription Prediction

## 📋 Project Overview

This project develops a predictive model for bank term deposit subscriptions, a critical application in financial services marketing. By analyzing customer demographic, financial, and campaign interaction data, the model identifies clients most likely to subscribe, achieving an impressive **F1 score of 0.945**. This demonstrates strong predictive capability for this imbalanced classification task.

## 📊 Dataset Description

### Source
The project uses the **Bank Marketing Dataset** (`bank-full.csv`) containing 45,211 records with 16 features.

### Features
The dataset includes three main categories of customer information:

**Demographic Features:**
- `age`: Customer's age
- `job`: Type of job
- `marital`: Marital status
- `education`: Education level
- `default`: Has credit in default?
- `housing`: Has housing loan?
- `loan`: Has personal loan?

**Financial Features:**
- `balance`: Average yearly balance

**Campaign-Related Features:**
- `contact`: Contact communication type
- `day`: Last contact day of the month
- `month`: Last contact month of year
- `duration`: Last contact duration (removed due to data leakage concerns)
- `campaign`: Number of contacts performed during this campaign
- `pdays`: Number of days since last contact from previous campaign
- `previous`: Number of contacts performed before this campaign
- `poutcome`: Outcome of previous marketing campaign

**Target Variable:**
- `y`: Has the client subscribed to a term deposit? (yes/no)

## 🔧 Technical Implementation

### Libraries Used
- **pandas, numpy**: Data manipulation and numerical operations
- **matplotlib, seaborn**: Data visualization
- **scikit-learn**: Machine learning models and evaluation metrics
- **SHAP**: Model interpretability and feature importance analysis

### Data Preprocessing Steps

1. **Data Loading & Initial Inspection**
   - Loaded dataset with semicolon delimiter
   - Removed `duration` column (potential data leakage)
   - Checked for missing values and duplicates

2. **Feature Engineering**
   - Created `age_group` categories: Teen (<20), Young (20-34), Men (35-59), Old (≥60)
   - Created `week_group` from `day` feature: Week 1, Week 2, Week 3, Week 4
   - Dropped original `age` and `day` columns after feature engineering

3. **Data Cleaning**
   - Removed extreme outliers from `balance`, `pdays`, and `campaign` features
   - Eliminated 1,720 rows (3.8% of data) using percentile-based outlier detection

### Exploratory Data Analysis (EDA)

#### Target Variable Distribution
- **No subscription**: 88.3% (39,906 customers)
- **Subscription**: 11.7% (5,289 customers)
- **Class imbalance**: Significant with subscription being the minority class

#### Key Conversion Rate Insights

**Highest Converting Groups:**
- **Age Group**: Teens (39.1%), Old (33.5%)
- **Job**: Students (28.3%), Retired (22.6%)
- **Previous Outcome**: Success (64.5%)
- **Contact Type**: Cellular (14.7%)
- **Housing Loan**: No (16.6%)

**Lowest Converting Groups:**
- **Job**: Blue-collar (7.3%)
- **Marital Status**: Married (10.1%)
- **Contact Type**: Unknown (4.1%)

## 🤖 Model Development

### Algorithm
- **Random Forest Classifier**: Selected for its robustness with imbalanced data and ability to capture complex feature interactions

### Model Performance
- **F1 Score**: 0.945 (demonstrating excellent precision-recall balance)
- The high F1 score is particularly impressive given the class imbalance in the dataset

### Model Interpretability
- **SHAP (SHapley Additive exPlanations)**: Used to interpret model predictions and understand feature importance
- Provides insights into which factors most influence subscription likelihood

## 📈 Business Impact

### Marketing Optimization
1. **Resource Allocation**: Focus marketing efforts on high-potential customer segments
2. **Campaign Efficiency**: Reduce unnecessary contact costs by avoiding low-probability customers
3. **Conversion Rate Improvement**: Increase overall subscription rates through targeted approaches

### Strategic Insights
- **Demographic Targeting**: Prioritize students, retired individuals, and younger/older age groups
- **Communication Strategy**: Prefer cellular contact over other methods
- **Risk Assessment**: Customers without housing loans show higher conversion rates
- **Historical Success**: Previous campaign success is the strongest predictor of future subscriptions

## 🚀 Future Enhancements

1. **Advanced Feature Engineering**
   - Create interaction features between key variables
   - Temporal features based on month and seasonality

2. **Model Improvements**
   - Experiment with gradient boosting methods (XGBoost, LightGBM)
   - Implement more sophisticated handling of class imbalance
   - Ensemble methods for improved robustness

3. **Deployment Features**
   - Real-time prediction API
   - Integration with CRM systems
   - A/B testing framework for campaign optimization
   
---

## 🏆 Key Achievements

1. **High Predictive Accuracy**: F1 score of 0.945 demonstrates excellent model performance
2. **Actionable Insights**: Clear identification of high-conversion customer segments
3. **Business-Ready Solution**: Direct applicability to bank marketing operations
4. **Robust Methodology**: Comprehensive data preprocessing, feature engineering, and model validation

**Note**: This project successfully demonstrates how machine learning can drive tangible business value in the banking sector by optimizing marketing strategies and improving campaign ROI.
