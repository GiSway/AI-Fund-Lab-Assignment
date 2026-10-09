
# SC5001 Lab Assignment 1
## Part 2: Applied Machine Learning with AI Copilot

### Project Overview

This repository contains the Google Colab notebook for Part 2 of SC5001 Lab Assignment 1.

The objective of this experiment is to explore and compare Linear Regression and Ridge Regression using the California Housing dataset. The experiment also examines how feature scaling, cross-validation, and different regularisation strengths affect machine learning model performance.

Generative AI (GenAI) was used as a learning assistant to clarify machine learning concepts, interpret experimental results, and support the learning process.

## 1. Dataset

**Dataset:** California Housing Dataset

**Source:** Scikit-Learn (`fetch_california_housing`)

The dataset contains eight numerical input features used to predict median house values.

| Feature | Description |
|---|---|
| MedInc | Median income |
| HouseAge | Median house age |
| AveRooms | Average number of rooms |
| AveBedrms | Average number of bedrooms |
| Population | Population |
| AveOccup | Average household occupancy |
| Latitude | Geographic latitude |
| Longitude | Geographic longitude |

**Target Variable:** `MedHouseVal` (Median House Value)

## 2. Machine Learning Models

Two regression models were evaluated:

- **Linear Regression:** Establishes a baseline for predicting median house values.
- **Ridge Regression:** Extends Linear Regression by applying L2 regularisation to reduce the magnitude of model coefficients.

Feature scaling using `StandardScaler` was applied to standardise numerical features, particularly to ensure that Ridge regularisation treats features with different measurement scales appropriately.

## 3. Model Evaluation

Model performance was evaluated using **5-Fold Cross-Validation**, with the R² score as the evaluation metric.

Ridge Regression was tested using three different regularisation strengths (`alpha` values): 0.1, 10, and 1000.

### Experimental Results

| Model | Mean 5-Fold R² Score |
|---|---:|
| Linear Regression | 0.6457 |
| Ridge Regression (α = 0.1) | 0.6457 |
| Ridge Regression (α = 10) | 0.6443 |
| Ridge Regression (α = 1000) | 0.3574 |

### Key Findings

- Linear Regression and Ridge Regression with α = 0.1 achieved almost identical performance.
- Ridge Regression with α = 10 showed a slight decrease in R² score, suggesting that moderate regularisation had limited impact on predictive performance.
- Ridge Regression with α = 1000 performed significantly worse because excessive regularisation restricted the model's ability to learn important relationships, resulting in underfitting.
- The experiments demonstrate the importance of balancing model complexity and regularisation strength to achieve good generalisation.

## 4. Generative AI Assistance

GenAI was used to support the learning process in the following areas:

- Identifying the input features and target variable in the California Housing dataset.
- Understanding why feature scaling is important in regression models.
- Explaining the differences between Linear Regression and Ridge Regression.
- Understanding why 5-Fold Cross-Validation provides a more reliable performance estimate than a single train/test split.
- Interpreting how different Ridge alpha values influence model performance.
- Clarifying the concepts of underfitting, overfitting, and regularisation.

## 5. Tools and Libraries

- Python
- Google Colab
- Scikit-Learn
- Pandas
- Matplotlib
- Generative AI (ChatGPT, Gemini)

## 6. How to Run the Notebook

1. Download the `.ipynb` file from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Select **File → Upload notebook** and upload the downloaded file.
4. Ensure the required Python libraries are available.
5. Select **Runtime → Run all** to execute the notebook.
6. Review the model evaluation results and visualisations.

## 7. Repository Contents

```text
AI-Fund-Lab-Assignment/
│
├── SC5001_Lab_Assignment_1.ipynb
└── README.md
```

The notebook contains the Python implementation, model evaluation, and experimental results for Part 2 of the assignment.

## 8. Conclusion

The experiment demonstrates how regularisation affects regression model performance. Linear Regression and Ridge Regression with a small alpha value achieved comparable R² scores, while an excessively large alpha value caused significant underfitting.

Overall, the experiment highlights the importance of feature scaling, cross-validation, and choosing an appropriate regularisation strength when developing regression models.

## Authors
Khant Zay Hein

## Course: SC5001 - NTU
