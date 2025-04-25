# ml-sms-spam-detector
An end-to-end machine learning project that detects SMS spam using text preprocessing, model training, and a Streamlit-powered web interface.

# 📩 SMS Spam Detection

## 🧠 Overview
**SMS Spam Detection** is a machine learning-powered web application that takes a text message (SMS) as input and predicts whether it's a **spam** or **ham** (not spam). The app is built using **Python** and deployed on the web using **Streamlit**, making it simple and accessible for end users.

---

## 📌 Table of Contents
- [Overview](#-overview)
- [Technologies Used](#-technologies-used)
- [Features](#-features)
- [Dataset](#-dataset)
- [Data Preprocessing](#-data-preprocessing)
- [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [Model Building](#-model-building)
- [Web Deployment](#-web-deployment)
- [Demo](#-demo)
- [Installation](#-installation)
- [Usage](#-usage)
- [Contributions](#-contributions)
- [License](#-license)

---

## 🛠️ Technologies Used
- Python 🐍
- Scikit-learn 🔬
- Pandas 🧼
- NumPy 🧮
- Streamlit 🌐
- Matplotlib & Seaborn 📊
- NLTK (for text processing)

---

## ✨ Features
- 📥 Import and handle real SMS spam dataset
- 🧹 Perform text preprocessing and cleaning
- 📊 Visualize data with bar charts, pie charts, word clouds, and heatmaps
- 🤖 Train multiple machine learning classifiers
- ✅ Choose the best model based on performance metrics
- 💻 User-friendly Streamlit web interface for real-time predictions

---

## 📚 Dataset
- **Name**: SMS Spam Collection
- **Source**: [Kaggle - SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
- **Size**: 5,500+ labeled SMS messages (`ham` or `spam`)
- **Format**: CSV

---

## 🔍 Data Preprocessing
- Removed null and duplicate entries
- Converted all messages to lowercase
- Tokenized the messages into words
- Removed:
  - Punctuation
  - Stop words (common English words like "and", "is", "the")
  - Special characters
- Applied **stemming** using NLTK’s Porter Stemmer
- Encoded the target label (`ham` → 0, `spam` → 1)

---

## 📈 Exploratory Data Analysis (EDA)
- Checked class distribution (`ham` vs `spam`)
- Counted characters, words, and sentences in each message
- Generated:
  - **Bar plots** and **Pie charts** for visualizing spam vs ham ratios
  - **WordClouds** for frequently used words in spam and ham
  - **Heatmaps** for correlation analysis
  - **Five number summary** (min, Q1, median, Q3, max)

---

## 🧠 Model Building
Tested multiple classification algorithms:
- Logistic Regression
- Naive Bayes
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Support Vector Classifier (SVC)
- Extra Trees Classifier

🏆 **Best model** was selected based on performance metrics like **accuracy**, **precision**, and **F1 score**.  
Final model achieved **100% precision** in detecting spam messages.

---

## 🌐 Web Deployment
Deployed using **Streamlit** with a minimal and intuitive interface.  
User can enter a message and get an instant prediction (`Spam` or `Not Spam`) based on the trained model.

---

## 🎥 Demo
🔗 _[Insert your app URL or a video demo link here]_  
Example: https://sms-spam-detector.streamlit.app

---

## 💻 Installation
Install dependencies
Create a virtual environment (optional but recommended):

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows
Then install the requirements:

bash
Copy
Edit
pip install -r requirements.txt

Start the Streamlit app by running:

bash
Copy
Edit
streamlit run app.py
Open your browser and go to:
http://localhost:8501


