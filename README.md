# Email-Sms-Spam-Detector

Application link: https://email-sms-spam-detector-sxuq.onrender.com

A machine learning-based web application that classifies messages as Spam or Not Spam using Natural Language Processing (NLP). The model is trained on a labeled dataset of SMS messages and deployed using Streamlit.

📌 Features

✅ Text preprocessing using stopword removal & stemming
✅ TF-IDF Vectorization for text feature extraction
✅ Naïve Bayes Classification for message prediction
✅ User-friendly Web Interface using Streamlit
✅ Deployed on Render for easy access

📝 Dataset

The dataset used for training consists of labeled SMS messages, where:
ham represents non-spam messages.
spam represents unwanted promotional messages.
The dataset undergoes preprocessing, including:
Lowercasing
Tokenization
Stopword removal
Stemming
TF-IDF vectorization

🏗 Model Training & Deployment

🔹 1. Data Preprocessing

Convert text to lowercase.
Remove special characters and stopwords.
Apply stemming.

🔹 2. Feature Extraction

Use TF-IDF Vectorization to transform text into numerical data.

🔹 3. Model Training

Train a Multinomial Naïve Bayes Classifier using Scikit-learn.
Save the trained model and vectorizer using Pickle.

🔹 4. Deployment

Use Streamlit for the user interface.
Deploy on Render.

🙌 Acknowledgements

NLTK for text preprocessing
Scikit-learn for model training
Streamlit for UI development
Render for free hosting
