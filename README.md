# SMS-SPAM-CLASSIFIER
✅ Project Overview

SMS Spam Classifier is an NLP-based machine learning system designed to detect and classify mobile text messages as:

📩 Spam (Promotional / Fraud / Phishing)
✉️ Not Spam (Normal SMS)

The system uses a Naïve Bayes classifier with TF-IDF text vectorization and provides real-time message prediction.

Access is provided through:

🔹 Python script
🔹 Trained ML pipeline
🔹 Custom message input prediction

🔹 1. Spam Detection Model (Python – Scikit-Learn)
✅ Setup
cd spam_classifier
pip install -r requirements.txt

📥 Dataset

The dataset spam.csv includes 2 columns:

Column	Description
v1	Label (spam / ham)
v2	SMS message content
🧠 Training Workflow

Clean & preprocess dataset

Convert text to numerical format using

CountVectorizer

TF-IDF Transformer

Train Multinomial Naïve Bayes classifier

Evaluate using classification metrics

🚀 Run the Program
python spamfilter.py

🔌 Core Prediction Function
def predict_spam(message):
    prediction = pipeline.predict([message])
    return "Spam" if prediction[0] == 1 else "Not Spam"

🔗 Example Usage
print(predict_spam("Congratulations! You won a free iPhone, click here to claim"))
# Output → Spam

print(predict_spam("Meeting at 3 PM, don't be late"))
# Output → Not Spam

🔎 Model Evaluation

Outputs:

Accuracy Score

Precision / Recall / F1-Score

Confusion Matrix (optional)

Achieved Accuracy: ~96%

🔧 Tech Stack
Component	Tools
Language	Python
ML Library	Scikit-Learn
Data Handling	Pandas
NLP	CountVectorizer + TF-IDF
Algorithm	Multinomial Naïve Bayes
🌐 (Optional) API / Deployment Ideas

Future integration options:

FastAPI endpoint for spam checks

Flask / Streamlit UI for public input

Deployment on Render / Hugging Face Spaces
