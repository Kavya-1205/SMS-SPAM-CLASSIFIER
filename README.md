# 📩 SMS Spam Classification using Machine Learning

This project is an NLP-based Machine Learning model that classifies SMS messages as **Spam** or **Not Spam**.  
The system converts raw text messages into numerical features using **TF-IDF vectorization** and predicts categories using a **Multinomial Naïve Bayes classifier**, achieving **~96% accuracy**.

---

## 🚀 Features
- 🔍 Accurate spam vs. non-spam SMS prediction
- ✨ Real-time custom message input support
- 📊 Model evaluation included (precision, recall, f1-score)
- 📁 Clean ML pipeline (preprocess → train → predict)

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

## 📂 Project Structure
SMS-Spam-Classifier/
│── spamfilter.py # Main ML model script

│── spam.csv # Dataset (spam & ham messages)

│── requirements.txt # Python dependencies

└── README.md # Documentation

---

## ⚙️ Setup Instructions

### 🔧 Installation
```bash
git clone https://github.com/<your-username>/SMS-Spam-Classifier.git
cd SMS-Spam-Classifier
pip install -r requirements.txt

▶️ Run the Project
python spamfilter.py

🔎 Example Usage
print(predict_spam("Congratulations! You won a cash prize! Click here!"))
# Output: Spam

print(predict_spam("Class will start at 2 PM today."))
# Output: Not Spam

📊 Model Performance
| Metric     | Score                          |
| ---------- | ------------------------------ |
| Accuracy   | ~96%                           |
| Evaluation | Classification Report included |



### 🗂 Dataset
The dataset contains two types of SMS messages:

📌 **spam** → unwanted promotional / scam / phishing / lottery / marketing messages  
📌 **ham** → normal messages sent by known contacts or valid services  

📍 **Source:** *SMS Spam Collection Dataset*

