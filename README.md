# Book Sales Analysis | Pandas,Seaborn and Matplotlib

![1](https://github.com/user-attachments/assets/dbbe173d-10bc-4ed2-b3a2-cafd73ffe191)
![2](https://github.com/user-attachments/assets/ebfd52f3-f207-4195-8701-9a62852df229)

Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Dataset](#dataset)
4. [Analysis Techniques](#analysis-techniques)
5. [Visualizations](#visualizations)
6. [Model Inference and Results](#model-inference-and-results)

### Note
The machine learning models implemented in this project have not performed well and require further optimization.

## Introduction
This project aims to analyze the sales of best-selling books across various dimensions such as genre, author, language, and publication year. By leveraging data analysis and machine learning techniques, the project seeks to uncover trends, patterns, and insights in book sales data.

## Project Overview
The Book Sales Analysis project utilizes a dataset containing information about best-selling books, including their titles, authors, genres, sales figures, and publication details. The analysis aims to answer key questions about sales trends, popular genres, and factors influencing book sales.

## Dataset
The dataset used for this analysis includes the following columns:
- **Book**: Title of the book
- **Author(s)**: Author(s) of the book
- **Original Language**: Language in which the book was originally published
- **First Published**: Year the book was first published
- **Approximate Sales in Millions**: Estimated sales figures
- **Genre**: Genre classification of the book

## Analysis Techniques
The project employs various data analysis techniques, including:
- Descriptive statistics to summarize the data
- Data visualization to illustrate trends and patterns
- Machine learning models to predict book sales and classify genres


## Visualizations
The analysis includes several visualizations to help interpret the data:
- Bar charts to show sales trends over decades.
- Stacked bar charts to illustrate genre evolution.
- Line charts for sales predictions.

## Model Inference and Results

## Sales Prediction Model
Using the Random Forest Regressor for predicting book sales, we achieved a Root Mean Squared Error (RMSE) of approximately 17.96. This metric indicates the average difference between predicted and actual sales figures, with lower values suggesting better predictive accuracy.

**RMSE: 17.96**: This value shows that our model has a moderate level of prediction accuracy. Given the sales figures, a prediction error of approximately 18 million can be significant, highlighting areas for potential improvement in the model.

## Genre Classification Model
For genre classification, we evaluated our model's performance using precision, recall, and F1-score metrics across various genres. The classification report provides insights into how well the model is performing in predicting different genres:

| Genre                                         | Precision | Recall | F1-score | Support |
|-----------------------------------------------|-----------|--------|----------|--------|
| Autobiography                                 | 0.00      | 0.00   | 0.00     | 1      |
| Children's Literature                         | 0.00      | 0.00   | 0.00     | 2      |
| Children's fiction                            | 0.00      | 0.00   | 0.00     | 1      |
| Erotica                                      | 0.00      | 0.00   | 0.00     | 1      |
| Fantasy                                      | 1.00      | 0.50   | 0.67     | 4      |
| ...                                          | ...       | ...    | ...      | ...    |
| Unknown                                       | 0.27      | 1.00   | 0.43     | 9      |
| Young Adult novel, adventure, dystopian, sci-fi | 0.00      | 0.00   | 0.00     | 1      |

### Overall Accuracy
The model achieved an accuracy of **31%** across all genres.

### Macro Average:
- **Precision**: 0.06
- **Recall**: 0.07
- **F1-score**: 0.05

### Weighted Average:
- **Precision**: 0.18
- **Recall**: 0.31
- **F1-score**: 0.19

## Key Observations
- **Imbalanced Dataset**: The classification performance indicates a potential issue with class imbalance, where certain genres have significantly more examples than others. This imbalance likely impacted the model's ability to accurately predict less frequent genres.
  
- **Genre Performance**: The genre **Fantasy** showed the highest precision and recall, suggesting the model performs relatively well for this category compared to others. In contrast, most genres achieved a precision and recall of 0, indicating challenges in accurately predicting those classes.

- **Need for Improvement**: Given the results, further optimization strategies, such as oversampling minority classes, using different classification algorithms, or fine-tuning hyperparameters, may be necessary to improve classification performance across all genres.

## Conclusion
The analyses provide valuable insights into book sales trends and genre classification. While the sales prediction model demonstrates reasonable accuracy, the genre classification model shows significant room for improvement, primarily due to the imbalanced dataset and the complexity of genre categorization.

