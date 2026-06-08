# Titanic Survival Prediction using Machine Learning

## 📌 Project Overview

The Titanic Survival Prediction project is a machine learning classification application that predicts whether a passenger survived the Titanic disaster based on passenger information such as age, gender, ticket class, fare, and family details.

This project demonstrates the complete machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, model evaluation, and prediction generation.

---

## 🎯 Objective

To build a machine learning model capable of predicting passenger survival on the Titanic using historical passenger data.

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Joblib
* Jupyter Notebook

---

## 📂 Project Structure

```text
Titanic-Survival-Prediction/
│
├── data/
│   ├── train.csv
│   └── test.csv
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── predict.py
│
├── models/
│   └── random_forest.pkl
│
├── outputs/
│   └── submission.csv
│
├── notebooks/
│   └── Titanic_Project.ipynb
│
├── requirements.txt
├── README.md
└── report.pdf
```

---

## 📊 Dataset

Dataset Source:

* Kaggle Titanic: Machine Learning from Disaster

The dataset contains passenger information such as:

* Passenger ID
* Passenger Class (Pclass)
* Name
* Gender (Sex)
* Age
* Number of Siblings/Spouses (SibSp)
* Number of Parents/Children (Parch)
* Ticket Number
* Fare
* Cabin
* Embarked Port
* Survival Status (Target Variable)

---

## ⚙️ Project Workflow

### 1. Data Exploration

* Understanding dataset structure
* Checking missing values
* Visualizing feature distributions
* Identifying important features

### 2. Data Cleaning

* Handling missing Age values using median imputation
* Filling missing Embarked values using mode
* Filling missing Fare values
* Removing highly missing Cabin column

### 3. Feature Engineering

Created additional features:

* FamilySize
* IsAlone

These features improve model performance by providing additional information about passenger relationships.

### 4. Data Encoding

Converted categorical features into numerical values:

* Sex
* Embarked

### 5. Model Training

Implemented:

* Logistic Regression
* Random Forest Classifier

### 6. Hyperparameter Tuning

Used GridSearchCV to find optimal parameters for the Random Forest model.

### 7. Model Evaluation

Performance evaluated using:

* Accuracy Score
* Precision
* Recall
* F1 Score
* Confusion Matrix

### 8. Prediction Generation

Generated predictions for the test dataset and created a Kaggle-compatible submission file.

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Titanic-Survival-Prediction.git
```

Move into the project directory:

```bash
cd Titanic-Survival-Prediction
```

Install required packages:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### Train the Model

```bash
python src/train.py
```

This creates:

```text
models/random_forest.pkl
```

### Generate Predictions

```bash
python src/predict.py
```

This creates:

```text
outputs/submission.csv
```

---

## 📈 Model Performance

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | ~80%     |
| Random Forest       | ~85–88%  |

Random Forest achieved the best performance and was selected as the final model.

---

## 📋 Sample Features Used

```python
features = [
    'Pclass',
    'Sex',
    'Age',
    'SibSp',
    'Parch',
    'Fare',
    'Embarked',
    'FamilySize',
    'IsAlone'
]
```

---

## 🔍 Key Learnings

* Data Cleaning and Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Classification Algorithms
* Model Evaluation Metrics
* Hyperparameter Tuning
* Machine Learning Project Deployment Workflow

---

## 📸 Future Improvements

* Develop a Flask/Django web application
* Deploy the model online
* Experiment with XGBoost and LightGBM
* Improve feature engineering techniques
* Build an interactive prediction dashboard

---

## 👨‍💻 Author

Anurag

B.Tech Computer Science and Engineering

National Institute of Technology Jalandhar

---

## 📄 License

This project is intended for educational and learning purposes.
