# ❤️ Heart Stroke Prediction

A machine learning web app that predicts a person's risk of heart disease based on key clinical parameters — built with **Streamlit** and a **K-Nearest Neighbors (KNN)** classifier.

**🔗 Live App:** [heart-stroke-prediction-fxpderezgflg4rjya9xung.streamlit.app](https://heart-stroke-prediction-fxpderezgflg4rjya9xung.streamlit.app)

---

## 📌 Overview

Heart disease remains one of the leading causes of death worldwide. Early risk identification can help people seek timely medical attention. This project uses a supervised machine learning model trained on the **Heart Failure Prediction Dataset** to classify whether a person is at **low** or **high** risk of heart disease, based on 11 clinical input features.

---

## ✨ Features

- Interactive web interface — no coding or setup needed to use it
- Instant prediction with a single click
- Built on a KNN classifier trained on real clinical data
- Clean, minimal UI powered by Streamlit
- Fully deployed and publicly accessible

---

## 🧠 How It Works

1. The user enters clinical details through sliders and dropdowns
2. Inputs are one-hot encoded to match the model's training format
3. Numerical features are scaled using a fitted `StandardScaler`
4. The trained `KNeighborsClassifier` predicts the outcome
5. The app displays the result as **Low Risk** ✅ or **High Risk** ⚠️

---

## 📊 Input Parameters

| Feature | Description |
|---|---|
| Age | Age of the patient |
| Sex | M / F |
| Chest Pain Type | ATA, NAP, TA, ASY |
| Resting Blood Pressure | mm Hg |
| Cholesterol | mg/dL |
| Fasting Blood Sugar | > 120 mg/dL (1 = true, 0 = false) |
| Resting ECG | Normal, ST, LVH |
| Max Heart Rate | Beats per minute |
| Exercise-Induced Angina | Y / N |
| Oldpeak | ST depression induced by exercise |
| ST Slope | Up, Flat, Down |

---

## 🛠️ Tech Stack

- **Python**
- **Streamlit** — web app framework
- **scikit-learn** — model training (KNN, StandardScaler)
- **Pandas** — data preprocessing
- **Joblib** — model serialization

---

## 📂 Project Structure

```
Heart-Stroke-Prediction/
├── app.py               # Streamlit application
├── KNN_heart.pkl         # Trained KNN model
├── scaler.pkl             # Fitted StandardScaler
├── columns.pkl            # Expected feature columns (encoding order)
├── heart.csv              # Training dataset
├── requirements.txt        # Python dependencies
└── README.md
```

---

## 🚀 Run Locally

```bash
# Clone the repository
git clone https://github.com/SURAJ-SAW123/Heart-Stroke-Prediction.git
cd Heart-Stroke-Prediction

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

---

## 📈 Model Performance

Trained and evaluated on an 80/20 train-test split:

- **Accuracy:** ~85%
- **F1 Score:** ~0.87

---

## 📄 Dataset

This project uses the [Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction), a combination of five publicly available heart disease datasets.

---

## 👤 Author

**Suraj Saw**
B.Tech, Electrical and Electronics Engineering — Birla Institute of Technology, Mesra

---

## ⚠️ Disclaimer

This tool is for **educational and demonstrative purposes only** and is **not a substitute for professional medical advice, diagnosis, or treatment**. Always consult a qualified healthcare provider for medical concerns.
