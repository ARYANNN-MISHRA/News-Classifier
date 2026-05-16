# FAKE-NEWS-DETECTOR
📰 AI-Powered Fake News Detector
An interactive web application that uses BERT (Bidirectional Encoder Representations from Transformers) to classify news headlines or articles as Real or Fake with confidence scores.

🚀 Project Description
Misinformation is a growing challenge in the digital age. This project leverages a state-of-the-art Transformer-based NLP model (BERT) to analyze and classify news content contextually — going beyond simple keyword matching to understand the deeper semantics of the text.

🧠 How It Works

User inputs a news headline or article snippet
Text is tokenized using BertTokenizer with a max length of 512 tokens
Tokenized input is passed through BertForSequenceClassification
Softmax probabilities are computed for two classes: Real and Fake
Predicted label and confidence scores are displayed interactively


✨ Features

BERT-based contextual text classification
Real-time confidence scores for both Real and Fake classes
Clean Streamlit UI with visual progress indicators
Model caching with @st.cache_resource to prevent reloading on every interaction
Fun visual feedback — balloons for Real news, snow for Fake news


🛠 Tech Stack

Python
Streamlit
Hugging Face Transformers
PyTorch
NumPy


🚀 Run Locally
bashgit clone https://github.com/yourusername/fake-news-detector.git
cd fake-news-detector
pip install -r requirements.txt
streamlit run app.py

📦 Requirements
streamlit
torch
transformers
numpy

⚠️ Disclaimer
This app uses a base bert-base-uncased model without fine-tuning on a labeled fake news dataset. For production use, the model should be fine-tuned on a large, high-quality labeled dataset for reliable results.

🔮 Future Improvements

Fine-tune BERT on a dedicated fake news dataset
Add support for full article URL input
Deploy on Streamlit Cloud or Hugging Face Spaces
Integrate explainability (highlight which words influenced the prediction)
Add multilingual support


👤 Author
Aryan Mishra
