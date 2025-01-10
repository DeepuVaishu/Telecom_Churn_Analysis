# Churn Prediction Project

## Overview
This project focuses on predicting customer churn for a telecom company. Churn refers to customers discontinuing their service with the company. By building a machine learning model, we aim to identify at-risk customers and provide actionable insights for retention strategies.

## Objective
The primary objectives of this project are:
1. **Data Analysis**: Understand the factors influencing customer churn through exploratory data analysis (EDA).
2. **Feature Engineering**: Prepare the dataset for effective model training by selecting and transforming relevant features.
3. **Model Building**: Train multiple machine learning models and evaluate their performance to identify the best-performing model.
4. **Unseen Data Prediction**: Use the final model to predict churn on new, unseen data.

## Dataset
The dataset contains customer information, service usage, and account status. Key features include:
- **Numeric Features**: Account length, total minutes (day, evening, night), and total international minutes.
- **Categorical Features**: International plan, voice mail plan, and state.
- **Target Variable**: Churn (Yes/No).

### Class Imbalance
The dataset exhibits class imbalance, with significantly fewer churn cases compared to non-churn cases. To address this:
- SMOTE (Synthetic Minority Oversampling Technique) was applied during model training.

## Workflow
1. **Exploratory Data Analysis (EDA)**
   - Visualized distributions, correlations, and class imbalance.
   - Identified patterns and relationships between features and churn.

2. **Data Preprocessing**
   - Handled missing values and encoded categorical variables using `LabelEncoder`.
   - Standardized numeric features using `StandardScaler`.
   - Selected important features using `SelectKBest`.

3. **Model Training and Evaluation**
   - Models trained include:
     - Logistic Regression
     - Random Forest Classifier
     - Gradient Boosting Classifier
     - Decision Tree Classifier
     - Support Vector Machine (SVM)
     - Guassian NB
   - Evaluated using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.
   - Addressed class imbalance by applying SMOTE to the training data.

4. **Pipeline Implementation**
   - Built pipelines combining preprocessing, feature selection, SMOTE, and model training.
   - Ensured reproducibility and modularity.

5. **Prediction on Unseen Data**
   - Final model applied to unseen data for churn prediction.

## Key Results
- The best-performing model achieved:
  - **Accuracy**: 92 %
- Random Forest Classifier was identified as the most effective model based on evaluation metrics.

## Insights and Recommendations
1. **Key Factors Influencing Churn**:
   - Customers with international plans and high international call usage were more likely to churn.

2. **Retention Strategies**:
   - Focus on customers with international plans by offering better rates or personalized offers.
   - Enhance engagement with high-usage customers through loyalty programs.

## Conclusion
This project successfully identified key factors driving customer churn and developed a predictive model with actionable insights. By implementing the suggested strategies, the telecom company can reduce churn rates and improve customer satisfaction.

## Future Work
- Explore advanced techniques like deep learning for improved predictions.
- Incorporate additional customer feedback and behavioral data.
- Build real-time churn prediction systems.

## How to Run the Project
1. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the Jupyter Notebook for step-by-step analysis and model building.
3. Use the provided pipeline script to predict churn on new data.

## Files in the Repository
- `classification_project_1.ipynb`: Jupyter Notebook with all project steps.
- `README.md`: Project documentation.

For any questions or feedback, please contact deepthydevadasan@gmail.com.


