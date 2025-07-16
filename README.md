# ❤️ Heart Disease & Symptom Detection Web App

This Streamlit-based web application allows users to assess their **risk of heart disease** based on clinical parameters and check for possible conditions based on symptoms. It provides intuitive visualizations and the ability to **generate a personalized PDF report**.

---

## 📌 Features

- 🧠 **Heart Disease Risk Assessment** based on parameters like age, cholesterol, resting blood pressure, etc.
- 🔍 **Symptom Checker** that suggests possible medical conditions based on selected symptoms.
- 📊 **Data Visualizations** using Matplotlib and Seaborn for better understanding of risk factors.
- 📄 **PDF Report Generation** using FPDF including user input, predictions, and charts.
- 🎥 Demo Video Included: See the app in action (below).

---

## 🧪 Technologies Used

| Tech | Purpose |
|------|---------|
| `Streamlit` | Web UI and interactive elements |
| `NumPy`, `Pandas` | Data manipulation |
| `Seaborn`, `Matplotlib` | Visualization |
| `FPDF` | PDF generation |
| `Scikit-learn` | Model training and serialization |
| `Pickle` | Saving and loading trained model |

---

## 🏗️ App Structure

```bash
├── app.py                         # Streamlit app main file
├── train_and_save_model.py       # Script to train and save the Random Forest model
├── heart_disease_model.pkl       # Pre-trained model file
├── expanded_heart_disease_dataset.csv  # Dataset used for training
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation


🚀 How to Run the App
1. Clone the Repository
bash
Copy
Edit
git clone <your-repo-url>
cd Heart-disease-prediction-main

2. Create & Activate Virtual Environment (Optional but Recommended)
bash
Copy
Edit
python -m venv .venv
.venv\Scripts\activate  # On Windows


3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt

4. Run the App
bash
Copy
Edit
streamlit run app.py

🧠 Model Training
To retrain the model using your own data:

bash
Copy
Edit
python train_and_save_model.py
This will produce a new heart_disease_model.pkl.

📄 Sample Report Output
Once a user submits their data and symptoms, the app generates a custom PDF report containing:

Personal details

Risk level

Detected symptoms

Suggested conditions

Risk factor visualization chart

📂 Dataset
File: expanded_heart_disease_dataset.csv

Includes clinical features like age, cholesterol, thalach, oldpeak, etc.

target column indicates presence of heart disease.




