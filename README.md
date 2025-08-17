# Heart Disease Prediction App ❤️‍🩹

Welcome to my **very first Machine Learning project**! Built with **scikit-learn** (KNN) and powered by **Streamlit**, this app predicts the presence of heart disease based on user inputs—and benchmarks other models to see which performs best.  
Let’s dive in! 

---

##  Table of Contents
- [Motivation](#motivation)  
- [Features](#features)  
- [Project Structure](#project-structure)  
- [Installation & Setup](#installation--setup)  
- [Usage](#usage)  
- [Model Comparison & Evaluation](#model-comparison--evaluation)  
- [What I Learned](#what-i-learned)  
- [Future Work](#future-work)  
- [Contributing](#contributing)  
- [License & Disclaimer](#license--disclaimer)  

---

##  Motivation
Early prediction of heart disease can potentially support better health outcomes—and this project is a step toward that. It's also my chance to learn the full ML pipeline—from data preprocessing to frontend deployment.  

---

##  Features
- 🚀 **Streamlit UI** for interactive predictions  
- 🧠 **Primary Model**: KNN (scikit-learn)  
- ⚖️ **Model benchmarking**: Compared against Logistic Regression & Random Forest  
- 💾 **Model persistence** using `pickle`  
- 🔄 **Reproducible**—clone, install, and launch  

---

##  Project Structure
├── app.py                     # Streamlit interface  
├── model_train.py            # Data processing & model training  
├── heart_disease_model.pkl   # Serialized KNN model  
├── requirements.txt          # Project dependencies  
├── README.md                 # This file!  
└── data/
    └── heart.csv             # Dataset (download if not included)
## Installation & Setup

### Prerequisites
- Python 3.7 or higher  
- `pip` package manager  
- (Optional) Virtual environment tool (`venv` or `conda`)

### Installation Steps

git clone https://github.com/krishtewatia/Heart_Disease_Prediction.git
cd Heart_Disease_Prediction

# Optional: create a virtual environment
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows

pip install -r requirements.txt
Model Comparison & Evaluation
Model	Accuracy (Test Set)
Logistic Regression	~88 %
Random Forest	~90 %
K-Nearest Neighbors	~92 % (Best)

KNN came out on top after tuning—so it was selected for deployment!

What I Learned

Cleaning, encoding, and scaling medical data

Training, evaluating, and comparing classifier models

Tuning KNN (n_neighbors) for optimal performance

Saving models with pickle for quick reuse

Creating a clean, interactive UI with Streamlit

Building a full ML workflow—from data to UI

Future Work

Add hyperparameter tuning (GridSearchCV / RandomizedSearchCV)

Incorporate cross-validation for more reliable results

Introduce model interpretability tools like SHAP

Deploy to Streamlit Cloud, Heroku, or AWS

Polish the UI with validation, visuals, and improved layout

Contributing

Contributions are welcome! Just:

Fork the repo

git checkout -b feature-name

git commit -m "Add feature"

git push origin feature-name

Open a PR—happy to review!

License & Disclaimer

Licensed under MIT.

Disclaimer: This tool is for educational purposes only—not medical advice.
