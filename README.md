# Factors that Affect Heart Disease in Cleveland

## Introduction
Heart disease, affecting millions worldwide, includes conditions like arrhythmias, heart failure, and coronary artery disease. These conditions can lead to severe health issues, such as heart attacks and strokes. This project explores factors contributing to heart disease and aims to identify which factors have the most significant impact on predicting its presence within the Cleveland population.

**Predictive Question:**  
Is the Cleveland population likely to have heart disease based on age, resting blood pressure, cholesterol, maximum heart rate, and ST depression?

## Dataset
We used a dataset from the UCI Machine Learning Repository, containing data from hospitals in Cleveland and VA Long Beach. Key variables include:
- **Age** (years)
- **Resting blood pressure** (trestbps)
- **Cholesterol** (chol)
- **Maximum heart rate achieved** (thalach)
- **ST depression** induced by exercise (oldpeak)

These variables were selected based on research indicating their strong association with heart disease risk.

## Methodology
1. **Data Preprocessing**: The dataset was cleaned, with missing values handled, and labeled with meaningful column names.
2. **Exploratory Data Analysis**: We visualized each predictor to understand its distribution and relationships to heart disease.
3. **Modeling**: Using the k-nearest neighbors (KNN) classification, we determined the optimal `k` value for predicting heart disease presence. Cross-validation was applied to ensure model accuracy.
4. **Evaluation**: We tested the classifier with Cleveland and VA Long Beach data, analyzing its accuracy and visualizing the results.

## Findings
The model achieved an accuracy of approximately 65.8% with `k=66`. However, this accuracy is limited, likely due to an imbalance in classes and insufficient data size after filtering. Although the selected variables are generally associated with heart disease, they showed less predictive power than expected in this dataset.

## Discussion
While the model’s accuracy fell short of expectations, this project underscores the importance of data quality and balanced predictors in heart disease research. Our findings highlight that age and cholesterol, though significant, were not as predictive in our model, prompting further investigation into more complex or comprehensive datasets.

## Conclusion
Our project contributes insights into the limitations and potential of using specific health metrics for predicting heart disease. Future work could involve more robust datasets and a wider array of predictors to improve model reliability.
