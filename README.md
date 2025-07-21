# Employee Salary Prediction  
A machine learning project to predict salaries based on **age, experience, education level, gender, and job title**.  
Includes full data preprocessing, model training, evaluation, and a Streamlit app for deployment.

---

## Features  
- Data Cleaning & Preprocessing  
- Model Training and Comparison  
- Deployment using Streamlit  

---

## Project Structure  
- `Employee-Salary-Prediction.ipynb` → Complete ML pipeline  
- `Salary-Data.csv` → Dataset  
- `app.py` → Streamlit web application  
- `requirements.txt` → Python dependencies  

---

## How to Run  

### 1. Clone the repository  
```bash
git clone https://github.com/SatyamRanjan-404/Salary-Pridiction-ML-Modal
cd Employee-Salary-Prediction
```
### 2.Create a Virtual Environment
```
python -m venv .venv
# Activate on Windows
.\.venv\Scripts\activate
# Activate on macOS/Linux
source .venv/bin/activate
```
### 3.Install the Required Libraries
```
pip install -r requirements.txt
```
## Model Performance
| Model              | R² Score | MAE      | RMSE    |
|--------------------|---------:|---------:|--------:|
| Linear Regression  | 0.88     | 13,156   | 18,700  |
| Random Forest      | 0.98     | 3,037    | 7,724   |
| SVR                | 0.01     | 45,488   | 52,747  |
| Gradient Boosting  | 0.92     | 11,394   | 15,266  |

## Conclusion  
The **Random Forest Regressor** model achieved the best performance with an impressive **R² score of 0.98** and the lowest error metrics (**MAE, MSE, RMSE**) among all models tested.  

This indicates that:  
- The model explains **98% of the variance** in employee salaries.  
- Predictions are off by only **$3,500 on average (MAE)**.  
- The model effectively captures the relationships between employee attributes and their salaries.  

### Key factors influencing salary predictions include:  
- **Years of experience** (strongest positive correlation)  
- **Education level** (particularly advanced degrees)  
- **Job title** (specialized roles command higher salaries)  
- **Age** (moderate positive correlation)  

---

The **Streamlit app** provides an interactive interface to:  
- Explore these relationships visually  
- Compare model performances  
- Make real-time salary predictions based on user inputs  

---

## Tech Stack  
- **Python**: Core programming language  
- **Data Processing**: Pandas & NumPy  
- **Machine Learning**: Scikit-learn for preprocessing, model training, and evaluation  
- **Visualization**: Matplotlib & Seaborn for static plots  


