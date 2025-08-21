# Multilingual-Agricultural-Query-Classification-System
A multilingual AI system that classifies agricultural queries submitted in English, Hindi, or Gujarati into relevant categories using NLP and machine learning.

## Features
- Multilingual Support: Handles queries in English, Hindi, and Gujarati.
- Ensemble ML Models: Uses Naive Bayes, SVM, Logistic Regression, Random Forest, SGD, and XGBoost with voting strategies.
- High Accuracy: Achieved up to 71% F1-score (English), 68% (Hindi & Gujarati).
- Web Deployment: Flask-based app for real-time classification.
- Scalability: Designed to extend to more languages and advanced models like BERT, XLM-R.
- Farmer-Friendly: Classifies queries into 10 categories (e.g., Weather, Fertilizer, Government Schemes, Market Info).

  ---

## System Architecture
```mermaid
flowchart TD
    A["User Query (English / Hindi / Gujarati)"] --> B["Language Detection & Preprocessing"]
    B --> C["TF-IDF Vectorization"]
    C --> D["Ensemble Classifiers (SVM, RF, XGBoost, etc.)"]
    D --> E["Voting Mechanism (Hard/Soft)"]
    E --> F["Predicted Category"]
    F --> G["Flask Web Interface"]

├── data/                # Dataset (agricultural queries)
├── notebooks/           # Jupyter Notebooks for training & experiments
├── models/              # Saved ML models
├── app/                 
│   ├── app.py           # Flask web app
│   ├── static/          # CSS/JS files
│   └── templates/       # HTML templates
├── requirements.txt     # Dependencies
└── README.md  


This project is explained in the following video:

[Watch the explanation video](https://youtu.be/AcB2v6xQy5M)
