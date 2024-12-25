# Student Performance Predictor

## Author: Md Hasibul Haque Zahid  
## Student ID: 2302302  

---

### Project Description  
This project uses machine learning techniques to predict students' final grades in a nine-week online machine learning course. The dataset includes scores from quizzes, projects, and peer reviews, as well as interaction logs with the online platform. The primary goal is to provide accurate grade predictions, identify key performance indicators, and evaluate model performance.

Two supervised learning models, **Random Forest** and **Gradient Boosting**, were implemented and fine-tuned to achieve optimal results.

---

### Features  
- **Data Processing**:
  - Processed scores from quizzes, projects, and peer reviews.
  - Logs of student interaction with the platform were included for analysis.
  - Retained all features for model training after verifying no missing values.
- **Machine Learning Models**:
  - Random Forest with tuned hyperparameters:
    - `n_estimators = 200`
    - `max_depth = 10`
  - Gradient Boosting with tuned hyperparameters:
    - `n_estimators = 200`
    - `learning_rate = 0.1`
    - `max_depth = 5`
- **Performance Evaluation**:
  - Compared models using metrics like Mean Squared Error (MSE) and R² (coefficient of determination).
  - Visualized results through bar plots, residual plots, and predicted vs. actual plots.

---

### Dataset  
The dataset contains 107 student records with the following key features:
- **Quiz Scores** (e.g., `Week2_Quiz1`, `Week3_Quiz2`)
- **Mini-Project Scores** (e.g., `Week5_MP2`, `Week7_MP3`)
- **Peer Review Scores** (e.g., `Week5_PR2`)
- **Interaction Logs** (`Week1_Stat0` to `Week9_Stat3`)
- **Final Grades** (`Week8_Total` as the target variable)

The data was split into training (79.4%) and test (20.6%) sets for evaluation.

---

### Results and Insights  
- **Gradient Boosting** outperformed **Random Forest**:
  - Gradient Boosting achieved:
    - MSE: **0.0244**
    - R²: **0.9942**
  - Random Forest achieved:
    - MSE: **0.0395**
    - R²: **0.9906**
- **Important Features**:
  - Both models highlighted the importance of:
    1. `Week8_Total` (final grade of the previous week)
    2. `Week7_MP3` (Mini Project 3 score)
    3. `Week5_MP2` (Mini Project 2 score)
- Visualizations like bar plots and residual plots demonstrated Gradient Boosting's superior performance and predictive accuracy.

---

### Challenges and Solutions  
1. **Overfitting**:  
   - Adjusted hyperparameters to improve generalization.
2. **Complexity of Models**:  
   - Used feature importance analysis to interpret Gradient Boosting results.
3. **Evaluation Metrics**:  
   - Focused on MSE for a clearer understanding of prediction errors.

---

### Technologies Used  
- Python  
- Jupyter Notebook  
- Scikit-learn  
- Matplotlib  
- Pandas  

---

### Report  
A detailed report on the project is available [here](https://github.com/Xahidian/Student-Performance-Predictor/blob/main/Mini%20Project%202_Md%20Zahid.pdf). It provides an in-depth analysis of the dataset, modeling process, and results.

---

### Contact  
If you have any questions or would like to discuss the project further, feel free to reach out.  
Thank you for visiting my project!
