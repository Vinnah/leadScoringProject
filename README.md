Lead Scoring ML Project

A machine learning project to predict and rank potential customer leads based on their likelihood to convert. This project is designed to demonstrate key skills in EDA, model building, interpretability, automation, and dashboarding using public cloud platforms.

---

##  Project Structure

```
lead-scoring-ml/
├── data/                     # Input and output datasets
│   ├── leads.csv
│   ├── new_leads.csv
│   └── scored_leads.csv
├── models/                   # Saved models and scaler
│   ├── lead_model.pkl
│   └── scaler.pkl
├── notebooks/                # Jupyter notebooks
│   ├── 01_eda.ipynb
│   ├── 02_model_training.ipynb
│   ├── 03_shap_feature_importance.ipynb
│   ├── 04_batch_prediction.ipynb
│   └── 05_model_retraining.ipynb
├── app/                      # Streamlit app (coming soon)
│   └── streamlit_app.py
├── requirements.txt
└── README.md
```

---

##  Project Highlights

-  Clean, structured lead data with real-world-like features
-  EDA to explore conversion trends
-  Classification model using RandomForest
-  Label encoding and standard scaling
-  Evaluation: Confusion matrix, ROC curve, classification report
-  SHAP explainability for model transparency
-  Batch prediction notebook for scoring new leads
-  Retraining pipeline for future model updates
-  Deployment-ready (Streamlit Cloud + GitHub)

---

##  How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/lead-scoring-ml.git
   cd lead-scoring-ml
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch notebooks:
   ```bash
   jupyter lab
   ```

4.  Run Streamlit app:
   ```bash
   streamlit run app/streamlit_app.py
   ```

---

##  Sample Features in `leads.csv`

| Feature | Description |
|---------|-------------|
| `lead_source` | Marketing source (Google, LinkedIn, etc.) |
| `country` | Country of the lead |
| `browser` | Web browser used |
| `lead_age_days` | Days since the lead was created |
| `email_clicks` | Number of marketing email clicks |
| `form_submissions` | Number of contact form submissions |
| `visited_pricing_page` | Binary flag |
| `mobile_used` | Whether they visited on mobile |
| `industry` | Industry of the lead |
| `converted` | Target variable (1 = converted, 0 = not) |

---

##  Model Performance

| Metric | Value |
|--------|--------|
| Accuracy | ~0.85 |
| ROC-AUC  | ~0.91 |

*Note: Exact values may vary depending on random seed and data version.*

---

##  Tools & Technologies

- Python (Pandas, Scikit-learn, SHAP)
- Jupyter Notebooks
- Streamlit (for web app)
- joblib (for saving models)
- GitHub & GitHub Actions (for CI/CD)

---

##  Author

**Trécy Odede**  
[LinkedIn](https://www.linkedin.com/in/trecyodede) | [Portfolio](https://github.com/trecyodede)

---

##  Future Enhancements

- Streamlit dashboard with lead input form
- Google Sheets or CRM integration
- Auto retraining via GitHub Actions
- Flask or FastAPI backend for API deployment

