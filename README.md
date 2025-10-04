# Logistic Regression Model on Pima Indians Diabates

A beginner-level logistic regression model trained on the [Pima Indians Diabates](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database).

---

## About the dataset

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset.

The dataset contains the following columns:

- **Pregnancies**: Number of times pregnant
- **Glucose**: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- **BloodPressure**: Diastolic blood pressure (mm Hg)
- **SkinThickness**: Triceps skin fold thickness (mm)
- **Insulin**: 2-Hour serum insulin (mu U/ml)
- **BMI**: Body mass index (weight in kg/(height in m)^2)
- **DiabetesPedigreeFunction**: Diabetes pedigree function
- **Age**: Age (years)
- **Outcome**: Class variable (0 or 1) 268 of 768 are 1, the others are 0

In total there are **768** rows and **9** columns.

Here are the first few rows of the dataset:

| Pregnancies | Glucose | BloodPressure | SkinThickness | Insulin | BMI  | DiabetesPedigreeFunction | Age | Outcome |
|------------:|--------:|--------------:|--------------:|--------:|-----:|-------------------------:|----:|--------:|
| 6           | 148     | 72            | 35            | 0       | 33.6 | 0.627                   | 50  | 1       |
| 1           | 85      | 66            | 29            | 0       | 26.6 | 0.351                   | 31  | 0       |
| 8           | 183     | 64            | 0             | 0       | 23.3 | 0.672                   | 32  | 1       |
| 1           | 89      | 66            | 23            | 94      | 28.1 | 0.167                   | 21  | 0       |
| 0           | 137     | 40            | 35            | 168     | 43.1 | 2.288                   | 33  | 1       |

---

## About the Notebook

As mentioned the model was trained on logistic regression. The libraries `numpy`, `pandas`, `sklearn` and `os` were used in the process.

The notebook contains the following sections:

- **Import the libraries**
  
- **Load the dataset**

- **Define features and labels**: Based on the dataset, our label is the destinated *Outcome* while all the other columns being our features
  
- **Divide the datset into train and test**
  
- **Define and train the model**
  
- **Evaluation of the model through various metrics**

---

## Model Evaluation

The model achieves about **78%** accuracy and performs well at detecting negative cases, but it **misses many positive ones** (recall = 0.56), leading to a lower F1-score (0.65) for class 1. Overall, it’s **good at avoiding false positives but not as effective at finding all true positives**, so improving recall should be the main focus.

---

Build and trained on [Kaggle](https://www.kaggle.com) by Piyush Nagpal
