# 🧠 Customer Churn Prediction

This project predicts the likelihood of a bank customer leaving the service (churning), based on demographic and financial data. It uses a deep learning model built with TensorFlow and is deployed using Streamlit.

🔗 **Live App:**  
👉 https://customer-churn-wsuq6ij6o4y4bld7uh38fp.streamlit.app/

📂 **GitHub Repository:**  
👉 https://github.com/Devb1234/Customer-Churn

---

## 📌 Features

- Input customer attributes like age, salary, credit score, etc.
- Predicts **churn probability** using a trained neural network
- Built with:
  - TensorFlow
  - Pandas, NumPy, Scikit-learn
  - Streamlit for deployment

---

## 📊 Dataset

The project uses the **[Churn_Modelling.csv](https://github.com/Devb1234/Customer-Churn/blob/main/Churn_Modelling.csv)** dataset which includes the following features:

- `CreditScore`, `Geography`, `Gender`, `Age`, `Tenure`, `Balance`
- `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`
- Target: `Exited` (1 = churned, 0 = retained)

---

## 🏗️ Project Structure

```
.
├── app.py                      # Streamlit application
├── Churn_Modelling.csv         # Dataset
├── model.h5                    # Trained deep learning model
├── scaler.pkl                  # StandardScaler for features
├── onehot_encoder_geo.pkl      # OneHotEncoder for Geography
├── label_encoder_gender.pkl    # LabelEncoder for Gender
├── prediction.ipynb            # Notebook for model inference
├── experiments.ipynb           # Notebook for model training
├── requirements.txt            # Project dependencies
└── README.md                   # Project documentation
```

---

## 🚀 How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Devb1234/Customer-Churn.git
cd Customer-Churn
```

### 2. Create Conda Environment

```bash
conda create -p venv python=3.11 -y
conda activate ./venv
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch the App

```bash
streamlit run app.py
```

---

## 🧠 Model Overview

- **Model**: TensorFlow-based Deep Neural Network
- **Inputs**: Preprocessed numerical & categorical features
- **Preprocessing**:
  - `StandardScaler` for scaling
  - `LabelEncoder` and `OneHotEncoder` for categorical encoding
- **Output**: Binary classification (Churn / No Churn)

---

## 📎 Demo Screenshot

![Demo](https://placehold.co/600x400?text=Customer+Churn+App+Demo)

🔗 Try it live: https://customer-churn-wsuq6ij6o4y4bld7uh38fp.streamlit.app/

---

## 🙋‍♂️ Author

**Dev Bansal**  
📧 devbansal763@gmail.com  
📌 [GitHub - Devb1234](https://github.com/Devb1234)

---

## 📃 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
