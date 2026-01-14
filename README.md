# News Article Classification Using NLP and AWS

## 📌 Project Overview

This project implements a **multi-model news article classification system** using **Machine Learning, Deep Learning, and Transformer-based models**. The application classifies news articles into four categories: **World, Business, Sports, and Technology**. A **Streamlit web application** is used for interaction, and the solution is deployed on **AWS EC2**, with **AWS RDS** used for secure user login tracking.

This project was developed as part of an academic requirement to gain hands-on experience in **NLP, MLOps, and cloud deployment** using real-world datasets.

---

## 🎯 Objectives

* Build and compare ML, DL, and Transformer models for text classification
* Deploy a user-friendly Streamlit application
* Integrate AWS services (EC2, RDS, S3)
* Track user login activity securely
* Demonstrate end-to-end MLOps workflow

---

## 🧠 Models Used

### 1️⃣ Machine Learning Model

* **Algorithm:** Logistic Regression
* **Vectorization:** TF-IDF

### 2️⃣ Deep Learning Model

* **Architecture:** Embedding + LSTM + Dropout + Dense

### 3️⃣ Transformer Model

* **Model:** DistilBERT (Fine-tuned)
* **Library:** Hugging Face Transformers

---

## 📊 Model Evaluation

| Model Type  | Model Name          | Accuracy | F1-Score |
| ----------- | ------------------- | -------- | -------- |
| ML          | Logistic Regression | 0.88     | 0.87     |
| DL          | LSTM                | 0.90     | 0.89     |
| Transformer | DistilBERT          | **0.94** | **0.94** |

During testing, the Transformer-based model performed best in terms of accuracy and consistency across all article categories.

---

## 🗂 Dataset

* **Name:** AG News Topic Classification Dataset
* **Source:** Kaggle
* **Classes:** World, Business, Sports, Technology
* **Training Samples:** 120,000
* **Testing Samples:** 7,600

---

## 🖥 Application Features

* User login interface
* Article text input
* Model selection dropdown (ML / DL / Transformer)
* Category prediction with confidence score
* Cloud-based login tracking

---

## ☁ AWS Integration

### 🔹 EC2

* Hosts the Streamlit application

### 🔹 RDS

* Stores user login details:

  * Username
  * Login timestamp
  * Selected model

### 🔹 S3

* Stores trained model artifacts

---

## 🛠 Tech Stack

* Python
* Scikit-learn
* TensorFlow / Keras
* Hugging Face Transformers
* Streamlit
* AWS EC2, RDS, S3

---

## ▶ How to Run

```bash
pip install -r requirements.txt
streamlit run app/app.py
```

---

## 📁 Repository Structure

```
news-article-classification-aws/
├── app/
├── models/
├── notebooks/
├── data/
├── requirements.txt
└── README.md
```

---

## 📌 Notes

* Models are loaded dynamically for inference
* Secure database connection is used for RDS

---

## 🏁 Conclusion

This project demonstrates a complete NLP pipeline from data preprocessing to cloud deployment. By comparing traditional ML, deep learning, and transformer-based approaches, the system highlights the effectiveness of modern transformer models for text classification tasks.

---

> This project was developed and tested individually for learning and academic submission purposes.
