<div align="center">
	<h1>🩺 MediScan AI: Breast Cancer Detection</h1>
	<p><b>B.Tech CSE 5th Semester Project</b></p>
	<p><b>Invertis University, Bareilly (2025)</b></p>
	<p><b>Submitted by: <span style="color:#4f46e5;font-weight:bold">Ayush Gangwar</span></b></p>
	<a href="https://cancerdetction.vercel.app" target="_blank"><img src="https://img.shields.io/badge/Live%20Demo-Vercel-4f46e5?logo=vercel" alt="Live Demo"></a>
	<br><br>
</div>

---

## 📑 Abstract
This project is developed as a part of my B.Tech CSE 5th semester at Invertis University, Bareilly. It presents a complete pipeline for breast cancer detection using machine learning, covering data analysis, model building, evaluation, and a user-friendly web application for real-time predictions. The aim is to assist healthcare professionals in early and accurate diagnosis of breast cancer using the Wisconsin Diagnostic dataset, and to demonstrate practical ML deployment skills as a student project.

**Dataset:** [Wisconsin Diagnostic Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)

---

## ✨ Features
- 📊 **Interactive EDA**: Visualize feature relationships, class balance, and correlations
- 🏗️ **Robust ML Pipeline**: Imputation, scaling, SMOTE, RandomForest, GridSearchCV
- 📈 **High Accuracy**: >97% test accuracy, strong ROC AUC
- 🖥️ **Web App**: Upload CSV, manual entry, batch prediction, and instant results
- 🌗 **Modern UI**: Responsive, dark/light mode, modals, and professional design
- 📝 **API Endpoints**: `/predict`, `/predict_batch`, `/model_info`, `/health`
- 🧑‍💻 **Easy Deployment**: Ready for Vercel, Render, or local use

---

## 📦 File Structure
```
├── api/                  # Flask app for Vercel (index.py, static/, templates/)
├── cancer_model_notebook.ipynb  # Full ML pipeline notebook
├── data.csv              # Dataset (Wisconsin Breast Cancer)
├── arya_best_cancer.joblib      # Trained model (local use)
├── requirements.txt      # Python dependencies
├── README.md             # This file
└── ...
```

---

## 🛠️ Setup & Usage

### 1. Notebook (ML Pipeline)
```bash
# (Recommended) Create a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook cancer_model_notebook.ipynb
```

### 2. Web App (Flask/Vercel)
- For local Flask: Move `api/index.py` to root as `app.py`, ensure model file is present, and run:
```bash
python app.py
```
- For Vercel: Use the provided `api/` structure and deploy with Vercel CLI.

---

## 🌐 Live Demo
- **Vercel:** [cancerdetction.vercel.app](https://cancerdetction.vercel.app)

---

## 🔌 API Endpoints
| Endpoint         | Method | Description                       |
|------------------|--------|-----------------------------------|
| `/predict`       | POST   | Predict single case (form data)   |
| `/predict_batch` | POST   | Batch predict (CSV upload)        |
| `/model_info`    | GET    | Model metadata & performance      |
| `/health`        | GET    | Health check                      |

---

## 📊 Model Performance
- **Accuracy:** ~97.4%
- **Precision:** ~98.6%
- **Recall:** ~96.5%
- **ROC AUC:** ~0.996

---


---

## 🙏 Acknowledgements
- Project by Ayush Gangwar (2025), B.Tech CSE 5th Sem, Invertis University, Bareilly
- Special thanks to my faculty, friends, and open-source contributors for their support and guidance
- Dataset: UCI ML Repository
- ML: scikit-learn, imbalanced-learn, pandas, numpy
- Web: Flask, Vercel
- UI: Custom HTML/CSS/JS

---

## 📄 License
MIT License. See [LICENSE](LICENSE).
