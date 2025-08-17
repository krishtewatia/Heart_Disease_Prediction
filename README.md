# Heart Disease Prediction App

A beginner-friendly **Machine Learning project** for predicting heart disease. Built using **Scikit-learn's K-Nearest Neighbors (KNN)** and deployed via **Streamlit**, this app also benchmarks other models to identify the most accurate one. This marks my very first ML project — a complete end-to-end journey from data processing to UI deployment.

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
Predicting heart disease early can potentially support healthcare decisions. This project demonstrates how machine learning can contribute to this domain and serves as my introduction to the entire ML workflow—from dataset preprocessing to deployment.

---

##  Features
- **Interactive UI** built with **Streamlit**
- **Primary Model**: KNN classifier via `scikit-learn`
- **Benchmarking** against Logistic Regression, Random Forest, and optionally others
- **Model persistence** using `pickle` for fast deployability
- Fully reproducible — clone the repo, install dependencies, and launch

---

##  Project Structure
```text
├── app.py                     # Streamlit interface
├── model_train.py            # Script: data preprocessing & model training
├── heart_disease_model.pkl   # Serialized KNN model
├── requirements.txt          # Dependencies list
├── README.md                 # Project documentation
└── data/
    └── heart.csv             # Original dataset (download separately if needed)


---

Installation & Setup

Clone the repository

git clone https://github.com/krishtewatia/Heart_Disease_Prediction.git
cd Heart_Disease_Prediction


Install dependencies

pip install -r requirements.txt


Download the dataset

If data/heart.csv isn’t included, download from the UCI Heart Disease dataset or Kaggle (search “heart disease UCI dataset”).

Usage

Training (optional if model already serialized):

python model_train.py


Launch the Streamlit app:

streamlit run app.py


Interact with the UI to input patient features and view prediction results.

Model Comparison & Evaluation

I evaluated multiple models to choose the best-performing one. Sample evaluation (accuracy on test set):

Model	Test Accuracy
Logistic Regression	~88 %
Random Forest	~90 %
KNN (chosen)	~92 %

KNN gave the best performance and was selected for deployment.

What I Learned

Data Preprocessing: Cleaning, encoding categorical features, and scaling numerical values

Model Training & Evaluation: Comparing classifiers using accuracy, precision, recall, and F1-score

Hyperparameter Tuning: Optimizing n_neighbors for KNN

Model Serialization: Saving trained models using pickle for fast reuse

Deployment: Creating a simple, interactive web app using Streamlit

Full ML Workflow: Gaining experience across data science stages—from preprocessing to user-facing interface

Future Work

Automate hyperparameter tuning using GridSearchCV or RandomizedSearchCV

Integrate cross-validation for more robust evaluation

Add explainability (e.g., SHAP) for result transparency

Deploy app to Streamlit Cloud, Heroku, or AWS

Enhance UI with input validation, styling, and graphs

Contributing

Contributions and feedback are welcome! If you'd like to contribute:

Fork this repository

Create a new branch: git checkout -b feature-name

Commit your improvements: git commit -m "Add feature"

Push: git push origin feature-name

Open a pull request and I’ll review promptly

License & Disclaimer

This project is released under the MIT License.
Disclaimer: This tool is for educational purposes only and is not intended for medical use.

Happy predicting!


---

###  Why This README Works
- It follows recommended structure — clear sections (Motivation, Usage, Results, etc.) per best practices :contentReference[oaicite:0]{index=0}.
- Clear instructions for installation, usage, and reproducibility — essential for data science projects :contentReference[oaicite:1]{index=1}.
- Encourages maintainability and collaboration with a simple Contributing section.
- Includes License and disclaimer — important when dealing with health-related predictions for clarity and ethics, aligning with README best practices :contentReference[oaicite:2]{index=2}.

Feel free to adjust metrics, dataset links, or code filenames to match your actual project files. Let me know if you'd like beginner-friendly badges, shields, or a rendered preview!
::contentReference[oaicite:3]{index=3}
