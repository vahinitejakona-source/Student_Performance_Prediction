# Student Performance Prediction using Machine Learning

##  Project Overview

This project implements an end-to-end Machine Learning workflow to analyze and predict student performance based on selected student-related factors.

The project follows a complete Machine Learning lifecycle, starting from problem understanding and data collection to exploratory data analysis, preprocessing, model training, evaluation, and model selection.

The project was developed as part of a Machine Learning internship project.

---

##  Problem Statement

Student performance can be influenced by various factors such as:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course

The objective of this project is to use these factors to build regression models that predict a student's overall performance score.

---

##  Dataset

**Dataset:** Students Performance in Exams

**Dataset Size:**
- 1,000 student records
- 8 original attributes

The dataset contains information related to students' demographic characteristics, parental education, lunch type, test preparation, and examination scores.

### Original Score Features

- Math Score
- Reading Score
- Writing Score

### Categorical Features Used for Prediction

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch
- Test Preparation Course

---

##  Target Variable

A new target variable called `PerformanceScore` was created using the average of the three examination scores:

```python
PerformanceScore = (Math Score + Reading Score + Writing Score) / 3

For example:

Math Score     = 72
Reading Score  = 72
Writing Score  = 74

PerformanceScore = (72 + 72 + 74) / 3
                  = 72.67

The resulting PerformanceScore ranges from 0 to 100.


---

🔄 Machine Learning Workflow

The project follows these major steps:

Understanding the Problem Statement
                ↓
          Data Collection
                ↓
         Data Validation
                ↓
Exploratory Data Analysis (EDA)
                ↓
       Data Pre-Processing
                ↓
          Model Training
                ↓
        Model Evaluation
                ↓
         Model Selection


---

🔍 1. Understanding the Problem

The project investigates the relationship between student-related factors and overall academic performance.

The goal is to build a regression model that can estimate the student's PerformanceScore from the selected input features.


---

📥 2. Data Collection

The Students Performance in Exams dataset was used for this project.

The dataset contains 1,000 records and 8 original columns.


---

 3. Data Checks

The following data validation checks were performed:

Dataset shape

Column names

Data types

Missing values

Duplicate records

Statistical summary

Categorical value distributions


These checks helped verify the quality and structure of the dataset before model development.


---

 4. Exploratory Data Analysis

Exploratory Data Analysis was performed to understand patterns and relationships in the data.

Visualizations Used

Performance Score distribution

Performance Score vs Gender

Performance Score vs Race/Ethnicity

Performance Score vs Parental Level of Education

Performance Score vs Lunch Type

Performance Score vs Test Preparation Course


These visualizations were used to understand how the selected factors relate to student performance.


---

⚙️ 5. Data Pre-Processing

The categorical input features were converted into numerical representations using One-Hot Encoding.

Input Features

Gender
Race/Ethnicity
Parental Level of Education
Lunch
Test Preparation Course

Target

PerformanceScore

The dataset was divided into training and testing sets using an 80:20 split.

80% → Training Data
20% → Testing Data


---

🤖 6. Machine Learning Models

Three regression algorithms were trained and evaluated:

1. Linear Regression

Used as a baseline regression model to model the relationship between the selected features and PerformanceScore.

2. Decision Tree Regression

Used to model potentially non-linear relationships between the input features and target.

3. Random Forest Regression

Used as an ensemble regression approach combining multiple decision trees.


---

📏 7. Model Evaluation

The models were evaluated using:

Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted values.

Lower MAE is better.

Root Mean Squared Error (RMSE)

Measures prediction error while giving greater importance to larger errors.

Lower RMSE is better.

R² Score

Measures how well the model explains variation in the target variable.

Higher R² is better.


---

📈 Model Performance

The following results were obtained on the test dataset:

Model	MAE	RMSE	R² Score

Linear Regression	10.490	13.402	0.162
Decision Tree	11.801	15.183	-0.075
Random Forest	11.488	14.825	-0.025



---

🏆 Model Selection

Based on the test-set evaluation results, Linear Regression was selected as the final model among the three evaluated models.

It achieved:

Lowest MAE: 10.490

Lowest RMSE: 13.402

Highest R² Score: 0.162


Therefore, Linear Regression provided the strongest performance among the evaluated models for predicting PerformanceScore using the selected features.


---

💡 Key Learning Outcomes

Through this project, I gained practical experience in:

Understanding a real-world Machine Learning problem

Data collection and validation

Exploratory Data Analysis

Data visualization

Handling categorical variables

One-Hot Encoding

Train-test splitting

Building regression pipelines

Training multiple Machine Learning models

Evaluating regression models

Comparing model performance

Selecting a model based on evaluation metrics



---

🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab

Jupyter Notebook



---

📁 Project Structure

Student_Performance_Prediction/
│
├── Student_Performance_Prediction.ipynb
│
└── README.md


---

🚀 Future Improvements

The project can be further enhanced by:

Testing additional regression algorithms

Performing hyperparameter tuning

Applying cross-validation

Engineering additional meaningful features

Comparing different preprocessing strategies

Increasing the amount and diversity of training data

Deploying the final model as a web application or API



---

📌 Conclusion

This project demonstrates a complete Machine Learning workflow, from raw student data to model evaluation and selection. Multiple regression algorithms were compared using MAE, RMSE, and R² Score, with Linear Regression achieving the strongest test-set performance among the evaluated models.

The project provided practical experience in transforming raw data into a structured Machine Learning solution and understanding how preprocessing, feature selection, model training, and evaluation contribute to the overall ML pipeline.


---

👩‍💻 Author

Kona Vahini Teja

Machine Learning | Python | Data Analysis | Artificial Intelligence
