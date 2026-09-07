# Bank Marketing Prediction Using Logistic Regression

## Objective

The objective of this project is to develop a Logistic Regression model to predict whether a bank customer will subscribe to a term deposit based on customer and banking information.

## Dataset

The dataset used in this project is the Bank Marketing dataset. It contains information about customers, including demographic characteristics, account information, and details related to the bank marketing campaign.

The target variable is `y`, which indicates whether the customer subscribed to a term deposit:

- `no` = Customer did not subscribe
- `yes` = Customer subscribed

## Methodology

The following steps were performed:

1. Loaded the Bank Marketing dataset.
2. Examined the dataset structure and dimensions.
3. Checked for missing values.
4. Checked for duplicate records.
5. Analyzed the distribution of the target variable.
6. Separated the input features and target variable.
7. Encoded the target variable into binary values.
8. Converted categorical features into numerical values using One-Hot Encoding.
9. Divided the dataset into training and testing sets using an 80:20 ratio.
10. Standardized the numerical features using StandardScaler.
11. Created a Logistic Regression model.
12. Trained the model using the training dataset.
13. Generated predictions using the testing dataset.
14. Evaluated the model using accuracy, precision, recall, and F1-score.
15. Generated and visualized the confusion matrix.
16. Examined the model coefficients.

## Data Preprocessing

The dataset contains both numerical and categorical features.

The target variable `y` was converted into binary values:

- `no` → `0`
- `yes` → `1`

Categorical features were converted into numerical features using One-Hot Encoding.

The numerical features were standardized using StandardScaler so that features with different numerical scales could be handled appropriately by the Logistic Regression model.

## Train-Test Split

The dataset was divided into:

- 80% training data
- 20% testing data

Stratified splitting was used to maintain the class distribution in the training and testing sets.

## Model

The machine learning algorithm used in this project is Logistic Regression.

Logistic Regression is a supervised learning algorithm commonly used for binary classification problems. In this project, it predicts whether a customer will subscribe to a term deposit or not.

## Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

## Results

The Logistic Regression model achieved the following results on the test dataset:

| Metric | Score | Percentage |
|---|---:|---:|
| Accuracy | 0.901581 | 90.16% |
| Precision | 0.647368 | 64.74% |
| Recall | 0.348771 | 34.88% |
| F1 Score | 0.453317 | 45.33% |

## Confusion Matrix

The confusion matrix obtained from the model was:

```text
[[7784  201]
 [ 689  369]]
