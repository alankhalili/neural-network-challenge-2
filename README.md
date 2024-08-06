# neural-network-challenge-2

# Employee Attrition Prediction

This project aims to predict employee attrition using machine learning models. The dataset contains various employee-related features, and the target variable is whether an employee will attrite or not.

## Table of Contents
- [Installation](#installation)
- [Data](#data)
- [Preprocessing](#preprocessing)
- [Conclusion](#conclusion)

## Installation

To get started with the project, clone the repository and install the required packages:

```bash
git clone <repository_url>
cd <repository_directory>
pip install -r requirements.txt

## Data

The dataset used in this project contains the following features:

	•	Age
	•	Attrition
	•	BusinessTravel
	•	Department
	•	DistanceFromHome
	•	Education
	•	EducationField
	•	EnvironmentSatisfaction
	•	HourlyRate
	•	JobInvolvement
	•	JobSatisfaction
	•	OverTime
	•	StockOptionLevel
	•	WorkLifeBalance
	•	YearsAtCompany
	•	YearsSinceLastPromotion
	•	YearsWithCurrManager

The target variable is Attrition, which indicates whether an employee has left the company (Yes) or not (No).

## Preprocessing

The preprocessing steps include:

	1.	Encoding Categorical Variables: Converting categorical variables into numeric format using one-hot encoding.
	2.	Handling Missing Values: Imputing or removing missing values as necessary.
	3.	Feature Scaling: Scaling numeric features using StandardScaler.


## Conclusion:

Q1 Is accuracy the best metric to use on this data? Why or why not?

A1 Collectively, precision, recall, and the F1 score should be used as a whole, especially if the cost of false positives and false negatives are different

Q2 What activation functions did you choose for your output layers, and why?
A2 I choose the softmax for the department because there were multiple departments that coudl have been selected.  For the Attrition, I selected a sigmoid because the prediction of attrition was either yes or no, which sigmoind is best suited.

Q3 Can you name a few ways that this model might be improved?
A3
  a.	Increase Dataset Size - Collect more data to provide the models with a more representative sample of the problem space.
	b.	Cross-Validation - Use cross-validation techniques to get a better estimate of the model’s performance and avoid overfitting.
	c.	Hyperparameter Tuning - Perform hyperparameter tuning on Random Forest and Gradient Boosting models to further improve performance.
	d.	Feature Engineering:  Explore creating new features or including more features into the model.
