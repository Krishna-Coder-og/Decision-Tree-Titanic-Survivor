# Titanic Survival Prediction using Decision Tree

## Project Overview
This project implements a Decision Tree Classifier to predict whether a passenger survived the Titanic disaster based on personal and travel details.

It demonstrates a complete machine learning workflow, including data preprocessing, model training, evaluation, visualization, and overfitting control.

---

## Objective
To build a machine learning model that predicts survival (Survived = 0 or 1) using features such as:

- Age  
- Gender  
- Passenger Class  
- Fare  
- Embarkation Port  

---

## Tech Stack
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Graphviz  

---

## Dataset
- Source: Titanic Dataset (Kaggle)  
- Description: Contains passenger details such as age, gender, class, fare, and survival status  

---

## Project Workflow

### 1. Data Loading
- Loaded dataset using pandas.read_csv()

### 2. Data Preprocessing
- Handled missing values:
  - Age column filled with median  
- Removed irrelevant columns:
  - Name  
  - Ticket  
  - Cabin  
- Encoded categorical variables:
  - Used pd.get_dummies() for One-Hot Encoding  

### 3. Feature Selection
- Input features stored in X  
- Target variable stored in y (Survived)  

### 4. Train-Test Split
- 80% training data  
- 20% testing data  

### 5. Model Training
- Used DecisionTreeClassifier()

### 6. Model Evaluation
- Evaluated using accuracy_score  

---

## Visualizations
- Feature Importance  
- Confusion Matrix  
- Decision Tree Visualization  

---

## Overfitting Analysis
- Compared training vs testing accuracy at different depths  
- Observed overfitting at higher depths  

---

## Pre-Pruning
Used:

DecisionTreeClassifier(max_depth=4, min_samples_split=10, min_samples_leaf=3)

---

## Results
- Baseline Accuracy: 75.41%  
- Pre-Pruned Accuracy: 81.56%  

---

## How to Run

### Clone Repository
git clone https://github.com/your-username/titanic-decision-tree.git  
cd titanic-decision-tree  

### Install Dependencies
pip install pandas numpy matplotlib scikit-learn graphviz  

### Run
python your_script_name.py  

---

## Author
Krishna Shankar Maurya
