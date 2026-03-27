# 🤖 AI Ethics Digital Twin System

An AI-powered digital twin simulation designed to model, detect, and predict ethical risks in automated systems using machine learning and formal verification.

---

## 📌 Overview

This project simulates a **digital twin environment** where workers interact with automated systems. It focuses on identifying and preventing ethical issues such as:

* Privacy violations (monitoring without consent)
* Lack of worker notification during automation
* Missing retraining support
* High-energy system usage without review

The system combines:

* 🧠 Machine Learning (risk prediction)
* ⚖️ Ethical auditing
* 🔍 Formal verification using Z3

---

## 🚀 Features

* ✅ Simulation of worker behavior in automated environments
* ✅ Detection of ethical violations
* ✅ AI model to predict ethical risk
* ✅ Environmental impact simulation (energy usage)
* ✅ Formal verification of ethical rules using Z3 solver
* ✅ Data visualization of audit results

---

## 🧱 Project Structure

```
ai-ethics-digital-twin/
│── our_code_for_ethics_report.ipynb
│── requirements.txt
│── README.md
```

---

## ⚙️ Installation

Clone the repository:

```
git clone https://github.com/your-username/ai-ethics-digital-twin.git
cd ai-ethics-digital-twin
```

Install dependencies:

```
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the Jupyter Notebook:

```
jupyter notebook
```

Open:

```
our_code_for_ethics_report.ipynb
```

---

## 🤖 AI Model

A **Random Forest Classifier** is used to predict ethical risks based on:

* Consent status
* Monitoring activity
* Automation impact
* Notification status
* Retraining availability

📊 The model achieves ~80%+ accuracy in predicting risk scenarios.

---

## ⚖️ Ethical Rules (Formal Verification)

We use the **Z3 Solver** to enforce key ethical constraints:

* 🚫 No monitoring without consent
* 📢 Workers must be notified if affected by automation
* 🎓 Retraining support must be provided
* 🌱 High-energy runs must trigger review

✔ If solver returns **UNSAT** → system satisfies ethical constraints
❌ If solver returns **SAT** → violation detected

---

## 📊 Example Outputs

* Worker audit summary
* Risk distribution
* Ethical violation breakdown
* Environmental audit results

---

## 🧠 Key Insight

This project demonstrates how **AI systems can move from detecting ethical violations to predicting and preventing them**, improving accountability in automated environments.

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Z3 Solver

---

## 📈 Future Improvements

* 🔹 Real-world dataset integration
* 🔹 Interactive dashboard (Streamlit)
* 🔹 Advanced ML models (XGBoost / Neural Networks)
* 🔹 Real-time monitoring system

---

## 👤 Author

**Humera Khan**
MSc Advanced AI, UCD
**Aisling wallace**

---

## ⭐ Acknowledgements

* NVIDIA Omniverse (concept inspiration)
* UCD School of Computer Science
* Responsible AI coursework

---

