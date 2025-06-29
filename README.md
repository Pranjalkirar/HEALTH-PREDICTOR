# Health Predictor using Decision Tree

A machine learning project that predicts the likelihood of a chronic disease based on lifestyle and health factors using a Decision Tree classifier.

## 📊 Dataset Features

- Age
- Gender
- Height_cm
- Weight_kg
- BMI
- Smoker (Yes/No)
- Exercise_Freq (None, 1-2 times/week, 3-5 times/week, Daily)
- Diet_Quality (Poor, Average, Good, Excellent)
- Alcohol_Consumption (None, Low, Moderate, High)
- Stress_Level (0–10)
- Sleep_Hours
- Target: Chronic_Disease (Yes/No)

## 🧠 Model

- **Algorithm:** DecisionTreeClassifier from `scikit-learn`
- Encodes categorical data using mapping
- Trained/tested using `train_test_split`
- Exported as `.joblib` model
- Visualized using `tree.export_graphviz`

## 🚀 How to Run

1. Install requirements:
   ```bash
   pip install -r requirements.txt

2. Open the Jupyter Notebook:

jupyter notebook health-predictor.ipynb
Run all cells to train, evaluate, and test the model.

3. Run all cells to train, evaluate, and test the model.

📈 Example Prediction

sample_data = pd.DataFrame([{
    'Age': 30,
    'Gender': 1,
    'Height_cm': 170,
    'Weight_kg': 65,
    'BMI': 22.5,
    'Smoker': 0,
    'Exercise_Freq': 3,
    'Diet_Quality': 2,
    'Alcohol_Consumption': 1,
    'Stress_Level': 5,
    'Sleep_Hours': 7
}])

prediction = model.predict(sample_data)
print("Predicted:", prediction[0])  # 0 = No, 1 = Yes

