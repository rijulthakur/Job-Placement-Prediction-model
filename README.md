# Job Placement Prediction Model

## Overview
An end-to-end machine learning web application that predicts whether 
a candidate will be placed or not placed based on academic performance, 
work experience, and employability test scores. Built using Logistic 
Regression and deployed as an interactive web application using 
Streamlit.

## Problem Statement
Campus placement outcomes depend on multiple academic and personal 
factors. This project applies supervised binary classification to 
predict placement likelihood, enabling data-driven insight into 
the factors that influence hiring decisions.

## Dataset Features (13-14 input variables)
- Gender
- SSC (10th grade) percentage and board
- HSC (12th grade) percentage, board and subject stream
- Undergraduate degree percentage and field of study
- Work experience (yes/no)
- Employability test percentage
- MBA percentage and specialization
- Target variable: Placed / Not Placed

## Methodology

### Logistic Regression
Logistic Regression is a supervised learning algorithm used for 
binary classification. It models the probability of a binary outcome 
using the sigmoid function: mapping any real-valued input to a value 
between 0 and 1. The decision boundary separates the two classes 
(Placed/Not Placed) by finding the optimal weights through maximum 
likelihood estimation.

### Exploratory Data Analysis (EDA)
Data was analysed using histograms and scatter plots (Matplotlib, 
Seaborn) to identify distributions, correlations and outliers before 
model training.

### Data Preprocessing
Categorical variables (Gender, Work Experience, Degree Type) were 
label-encoded. Missing values were handled and features were 
standardised prior to training using pandas and NumPy.

### Model Training and Evaluation
Data was split into training and test sets using scikit-learn's 
train_test_split. Model accuracy was evaluated using sklearn's 
accuracy_score metric.

### Model Deployment
The trained model was serialised using Python's Pickle library and 
integrated into a Streamlit web application (app.py), enabling 
real-time predictions through a browser-based user interface.

## Tech Stack
- Python
- Jupyter Notebook
- pandas, NumPy
- scikit-learn (LogisticRegression, train_test_split, accuracy_score)
- Matplotlib, Seaborn
- Pickle
- Streamlit
- Pillow (PIL)

## Project Type
End-to-end ML pipeline from raw data to deployed web application.

## Author
**Rijul Thakur**  
B.E. Computer Science and Engineering, Chitkara University (2019–2023)
