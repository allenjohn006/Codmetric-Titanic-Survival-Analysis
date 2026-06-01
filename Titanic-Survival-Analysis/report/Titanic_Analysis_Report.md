# Titanic Survival Analysis Report

**Author:** Allen John  
**Date:** June 2026  

---

## 1. Objective
The primary objective of this project is to analyze the historical Titanic dataset to identify and understand the core factors and demographic features that influenced a passenger's likelihood of survival during the disaster. 

## 2. Tools Used
To achieve the project objectives, the following data science and visualization stack was utilized:
- **Python**: Core programming language.
- **Pandas**: Used for data manipulation, ingestion, and aggregation.
- **NumPy**: Employed for numerical operations and handling arrays.
- **Matplotlib & Seaborn**: Utilized to create static, informative, and visually appealing statistical graphics.
- **Scikit-Learn**: Used for data preprocessing, specifically utilizing `LabelEncoder` for transforming categorical features into machine-readable numerical formats.

## 3. Project Workflow
The analysis followed a structured data science pipeline:
1. **Data Loading**: Ingested the training (`train.csv`) and testing (`test.csv`) datasets into Pandas DataFrames.
2. **Data Cleaning**: Addressed structural issues and dropped features with excessive missing data (e.g., the `Cabin` column, which was missing over 70% of its values).
3. **Missing Value Treatment**: 
   - Imputed missing `Age` values using the median age of the passengers.
   - Imputed missing `Embarked` values using the most frequent absolute port of origin (mode).
4. **Feature Encoding**: Converted categorical strings (`Sex` and `Embarked`) into integers securely using Scikit-Learn's explicit encoding methods.
5. **Exploratory Data Analysis (EDA)**: Conducted univariant and bi-variant analysis to understand distributions.
6. **Data Visualization**: Plotted graphs (count plots, bar plots, histograms, heatmaps) to uncover hidden correlations in the data.
7. **Insight Extraction**: Derived conclusive, data-backed findings addressing the project's objective.

## 4. Key Findings & Insights
The exploratory data analysis resulted in several strong predictors for survival:

- **Gender Was the Strongest Predictor**: Females had significantly higher survival rates compared to males. The "women and children first" protocol was clearly evident within the data.
- **Socio-Economic Class Matters**: First-class passengers survived much more often than second and third-class passengers. Third-class passengers suffered the highest casualty rates.
- **Age as a Determining Factor**: Children (especially under the age of 10) had notably better chances of survival.
- **Predictive Power**: Overall, passenger class (`Pclass`) and gender (`Sex`) emerged as the strongest predictors of survival when analyzed simultaneously.

## 5. Conclusion
Through systematic data processing and visual exploration, this analysis successfully highlights the demographic prioritization during the Titanic's evacuation. Features like gender, socio-economic status, and age dictate the survival probability distributions decisively.
