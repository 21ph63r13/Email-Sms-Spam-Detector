# Email-Sms-Spam-Detector

🔗 Live Demo

Check out the deployed app on Render: https://email-sms-spam-detector-sxuq.onrender.com

A machine learning-based web application that classifies messages as Spam or Not Spam using Natural Language Processing (NLP). The model is trained on a labeled dataset of SMS messages and deployed using Streamlit.

📂 Project Structure
Email-SMS-Spam-Detector/
│── app.py                # Streamlit web app
│── sms_spam_detection.ipynb # Jupyter Notebook (model training)
│── vectorizer.pkl        # TF-IDF vectorizer (saved model)
│── model.pkl             # Trained Naïve Bayes model
│── requirements.txt      # Dependencies
│── README.md             # Project Documentation


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

Tokenize text into individual words.

Remove non-alphanumeric characters.

Remove stopwords (common words that don’t add much meaning, e.g., "the", "is").

Apply stemming (reducing words to their root form, e.g., "running" → "run").

🔹 2. Feature Extraction (TF-IDF Vectorization)

After preprocessing, use Term Frequency-Inverse Document Frequency (TF-IDF) to convert text into a numerical representation:

Term Frequency (TF): Measures how frequently a term appears in a document.

Inverse Document Frequency (IDF): Reduces the importance of common words across multiple documents.

Using TfidfVectorizer from Scikit-learn, we transform the processed text into a feature matrix for model training.

🔹 3. Model Training

used Multinomial Naïve Bayes, a probabilistic algorithm effective for text classification tasks.

🔹 4. Deployment

Use Streamlit for the user interface.
Deploy on Render.

🙌 Acknowledgements

NLTK for text preprocessing

Scikit-learn for model training

Streamlit for UI development

Render for free hosting
