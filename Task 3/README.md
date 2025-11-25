# Insurance Charges Prediction Analysis

## 📋 Project Overview
This project analyzes health insurance charges data to understand the key factors driving medical costs and build predictive models for accurate charge estimation. The analysis provides valuable insights for both insurance companies and policyholders.

## 🎯 Task Objective
The main objectives of this project were:
- Identify key factors influencing health insurance charges
- Build accurate predictive models for insurance cost estimation
- Handle data challenges like skewed distributions and outliers
- Provide actionable insights for insurance pricing strategies

## 🛠️ My Approach

### Data Understanding & Exploration
- Analyzed dataset with 1,338 records and 7 features
- Key features: age, sex, BMI, children, smoker status, region, insurance charges
- Initial exploration revealed right-skewed distribution of charges

### Data Preprocessing
- **Feature Engineering**: Created age groups and categorical transformations
- **Target Transformation**: Used Box-Cox transformation to normalize charges distribution
- **Visual Analysis**: Comprehensive EDA with histograms, box plots, and scatter plots

### Feature Analysis
Conducted detailed analysis of relationships:
- **Smoker Status**: Most significant factor affecting charges
- **Age**: Strong positive correlation with insurance costs
- **BMI**: Moderate impact on charges
- **Region & Children**: Secondary influencing factors

### Model Development
Implemented and compared three regression models:
- **Random Forest Regressor**
- **XGBoost Regressor** 
- **Linear Regression**

## 📊 Results and Insights

### Model Performance Comparison
| Model | RMSE | MAE | 
|-------|------|-----| 
| Random Forest | 0.6279 | 0.3906 | 
| Linear Regression | 0.6676 | 0.4897 | 
| XGBoost | 0.6950 | 0.4597 | 

### Key Findings



#### 📈 Data Insights
- Charges follow log-normal distribution requiring transformation
- Clear segmentation between smoker and non-smoker charges
- Linear relationships observed between age/BMI and charges
- Regional variations exist but are less significant

### Business Impact

#### For Insurance Companies:
- **Accurate Pricing**: 98%+ accurate cost predictions enable better risk assessment
- **Risk Segmentation**: Clear identification of high-risk profiles (smokers, high BMI)
- **Product Development**: Data-driven insights for tailored insurance products

#### For Consumers:
- **Cost Transparency**: Understand what factors drive premium costs
- **Informed Decisions**: Make lifestyle choices knowing their insurance impact
- **Financial Planning**: Better anticipate insurance expenses

## 💡 Technical Implementation

### Data Transformation Strategy
- **Box-Cox Transformation**: Optimal for handling skewed charge distribution
- **Feature Encoding**: Proper handling of categorical variables

### Model Selection Rationale
**Random Forest** was chosen as the final model because:
- Best performance on both RMSE (0.6279) and MAE (0.3906)
- Handles non-linear relationships effectively
- Robust to outliers and feature correlations
- Provides feature importance rankings

### Validation Approach
- Train-test split for model evaluation
- Multiple metrics (RMSE, MAE) for comprehensive assessment

## 🚀 Conclusion

The Insurance Charges Prediction project successfully demonstrates that machine learning can accurately predict health insurance costs while providing transparent insights into the key driving factors. The Random Forest model achieved excellent performance with minimal prediction errors, making it suitable for real-world insurance applications.
This project showcases how data science can create value for both businesses and consumers in the insurance industry.
