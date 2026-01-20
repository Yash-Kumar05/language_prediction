# 🌍 Language Detection App using SimpleRNN

## 📌 Project Overview

This project is an **end-to-end Language Detection application** built using **SimpleRNN** and deployed with **Streamlit**.
It predicts the language of a given text among **17 languages** such as English, Hindi, French, Malayalam, Spanish, Tamil, Arabic, etc.

**Project Highlights:**

* Multi-class text classification
* Handling class imbalance
* Complete NLP pipeline (training → evaluation → deployment)
* Simple and interpretable RNN-based model

---

## 🧠 Model Architecture

The model is kept simple to focus on core concepts.

**Architecture:**

* Embedding Layer
* SimpleRNN Layer
* Dropout Layer
* Dense Softmax Output Layer

**Flow:**
Embedding → SimpleRNN → Dropout → Dense (Softmax)

**Why SimpleRNN?**

* Easy to explain (interview-friendly)
* Captures sequential text patterns
* Lightweight and fast for deployment

---

## 📊 Dataset Information

* **Source:** Kaggle – Language Detection Dataset
* **Total Languages:** 17
* **Total Samples:** 10,267
* **Columns:**

  * Text (input sentence)
  * Language (target label)

⚠️ Dataset is imbalanced, so **class weights** are used.

---

## 🚀 Model Performance

| Metric        | Value     |
| ------------- | --------- |
| Test Accuracy | **95.8%** |
| Test Loss     | **0.16**  |

Improved performance due to:

* Class weighting
* Early stopping
* Proper preprocessing

---

## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* Scikit-learn
* Streamlit
* NumPy, Pandas, Matplotlib, Seaborn

---

## 📁 Project Structure

```text
Language-Detection-RNN/
├── saved_model/
│   ├── simple_rnn_model.h5
│   └── tokenizer.pkl
├── eda.ipynb
├── prediction.ipynb
├── app.py
├── requirements.txt
└── readme.md
```

---

## ⚙️ Installation Steps

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Adi3042/Language-Detection-using-RNN.git
cd Language-Detection-using-RNN
```

### 2️⃣ (Optional) Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate        # Linux/Mac
venv\Scripts\activate           # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
streamlit run app.py
```

---

## 🧪 Example

**Input:**

```text
यह एक अच्छा दिन है
```

**Output:**

```text
Predicted Language: Hindi
Confidence: 0.98
```

---
