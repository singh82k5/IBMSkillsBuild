
# 🧠 Employee Income Predictor (ML Classifier)

This project is a **machine learning model** that predicts whether an employee earns **more than $50K or not**, based on demographic and employment-related features. It uses the **Adult Census Income dataset** and is built with **Python and Scikit-learn**, ready to run on **Google Colab**.

---

## 🚀 Features

- 🔍 Predicts income class: `>50K` or `<=50K`
- 🧼 Handles missing and categorical data
- ⚙️ Uses a **Random Forest Classifier**
- 📊 Includes model evaluation metrics
- ✅ Google Colab-compatible and beginner-friendly

---

## 📁 Dataset Used

The model is trained on a version of the **Adult Income Dataset**, which contains the following features:
- Age, Education, Occupation
- Marital Status, Hours per week
- Capital gain/loss
- Native country, Workclass, Gender, Race, etc.

---

## 🔧 Technologies Used

- Python 3
- pandas
- scikit-learn
- joblib
- Google Colab

---

## 📌 How to Run

1. Upload the dataset (`adult 3.csv`) to Colab:
   ```python
   from google.colab import files
   uploaded = files.upload()
   ```

2. Copy and run the code from your notebook (or script).

3. Evaluate the model and make predictions using sample input.

---

## 🧪 Sample Prediction

```python
new_employee = pd.DataFrame([{
    'age': 40,
    'workclass': 'Private',
    'fnlwgt': 170000,
    'education': 'Bachelors',
    'educational-num': 13,
    'marital-status': 'Married-civ-spouse',
    'occupation': 'Exec-managerial',
    'relationship': 'Husband',
    'race': 'White',
    'gender': 'Male',
    'capital-gain': 0,
    'capital-loss': 0,
    'hours-per-week': 50,
    'native-country': 'United-States'
}])

prediction = model.predict(new_employee)
print("Predicted Income Category:", prediction[0])
```

---

## 📊 Example Output

```
Predicted Income Category: >50K
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
