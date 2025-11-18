# 📩 SMS Spam Classification using Machine Learning

This project is an NLP-based Machine Learning model that classifies SMS messages as **Spam** or **Not Spam**.  
The system converts raw text messages into numerical features using **TF-IDF vectorization** and predicts categories using a **Multinomial Naïve Bayes classifier**, achieving **~96% accuracy**.

---

## 🚀 Features
- 🔍 Accurate spam vs non-spam SMS prediction
- ✨ Real-time custom message input support
- 📊 Model evaluation included (precision, recall, f1-score)
- 📁 Clean ML pipeline (preprocessing → training → prediction)

---

## 🧠 Tech Stack
| Category | Tools Used |
|---------|-------------|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Machine Learning | Scikit-Learn |
| NLP | CountVectorizer, TF-IDF |
| Algorithm | Multinomial Naïve Bayes |

---

## 🗂 Dataset
The dataset contains two categories of SMS messages:

📌 **spam** → unwanted promotional / lottery / scam / phishing / fraud / marketing SMS  
📌 **ham** → normal legitimate SMS from contacts, banks, and services

📍 **Source:** *SMS Spam Collection Dataset*

---

## 📂 Project Structure
SMS-Spam-Classifier/

│── spamfilter.py # Main ML model script

│── spam.csv # Dataset (spam & ham messages)

│── requirements.txt # Python dependencies

└── README.md # Documentation


---

## ⚙️ Setup Instructions

### 🔧 Installation


git clone https://github.com/Kavya-1205/SMS-Spam-Classifier.git
cd SMS-Spam-Classifier
pip install -r requirements.txt

▶️ Run the Project


python spamfilter.py


🔎 Example Usage
python

print(predict_spam("Congratulations! You won a cash prize! Click here!"))
# Output → Spam

print(predict_spam("Class will start at 2 PM today."))
# Output → Not Spam


📊 Model Performance
Metric	Score
Accuracy	~96%
Evaluation	Classification Report included

