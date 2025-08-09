# Heart Disease Prediction using Logistic Regression

This project is a **machine learning model** built using logistic regression to predict whether a person has heart disease based on medical attributes such as age, cholesterol level, blood pressure, and others.

## Project Overview
Heart disease remains a significant global health challenge, accounting for a large number of fatalities. The proactive prediction and early detection of this condition are essential for effective prevention and improved treatment strategies. This project harnesses a **Logistic Regression** model utilizing the **Heart Disease Dataset** to classify patients as having heart disease (`1`) or not (`0`), contributing to our understanding and management of this critical health issue.

## 📂 Dataset Overview
The dataset (`data.csv`) consists of **1,025 records** and includes **14 attributes** that provide valuable insights into patient health:

| Column      | Description |
|-------------|-------------|
| age         | Patient's age |
| sex         | Gender (1 = male, 0 = female) |
| cp          | Chest pain type (0-3) |
| trestbps    | Resting blood pressure (mm Hg) |
| chol        | Serum cholesterol (mg/dl) |
| fbs         | Fasting blood sugar (>120 mg/dl, 1 = true, 0 = false) |
| restecg     | Resting electrocardiographic results (0-2) |
| thalach     | Maximum heart rate achieved |
| exang       | Exercise-induced angina (1 = yes, 0 = no) |
| oldpeak     | ST depression induced by exercise |
| slope       | Slope of peak exercise ST segment (0-2) |
| ca          | Number of major vessels (0-4) colored by fluoroscopy |
| thal        | Thalassemia type (1-3) |
| target      | Diagnosis of heart disease (1 = present, 0 = absent) |

This well-structured dataset is advantageous for our analysis as it:
- ✅ Contains no missing values, ensuring the reliability of our findings.
- ✅ Features balanced target classes (526 positive cases and 499 negative cases), which fosters a fair training environment for the model.

## ⚙️ Technologies Used
We utilize robust technologies to support this project, including:
- Python 3, a powerful language for data analysis.
- Libraries such as Pandas and NumPy for efficient data management and numerical analysis.
- Scikit-learn, which offers a comprehensive toolkit for machine learning applications.
- Google Colab, enhancing our interactive coding experience.

## 🧠 Model Development
1. **Data Preprocessing**
   - The `target` column was removed to define the feature set `X`, with the target variable `Y` clearly set.
   - A thoughtful train-test split was implemented, with 80% of the data dedicated to training and 20% reserved for testing.

2. **Model Training**
   - We implemented a Logistic Regression model (`sklearn.linear_model.LogisticRegression`) that aligns well with our classification goals, utilizing the default solver (`lbfgs`) and adjusting `max_iter` as necessary to ensure convergence.

3. **Model Evaluation**
   - The model demonstrated an accuracy of approximately **85%** on the training set and **80%** on the test set, highlighting its potential effectiveness.

4. **Prediction Example**
   Here's how we can make predictions using the trained model:
   ```python
   input_data = (71, 0, 0, 112, 149, 0, 1, 125, 0, 1.6, 1, 0, 2)
   model.predict([input_data])  # Output: [1], indicating the presence of heart disease.
   ``` 

This construction fosters a constructive tone by emphasizing the project's significance, the thoughtful approach to data and model development, and the positive aspects of the dataset being analyzed.
 
