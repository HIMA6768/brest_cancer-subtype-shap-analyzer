# 🧬 Breast Cancer Subtype & SHAP Intelligence Dashboard

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://brestcancer-subtype-shap-analyzer-himadri6768.streamlit.app/)

A cloud-connected Streamlit dashboard that fetches live patient data from Azure Cosmos DB, runs an XGBoost model for breast cancer subtype classification, performs SHAP analysis to identify the most effective genes, and generates an automated clinical executive report.

## 🔗 Live Application
You can access the live web application here:  
👉 Breast Cancer Subtype SHAP Analyzer]   (https://brestcancer-subtype-shap-analyzer-himadri6768.streamlit.app/)
 
## 🚀 Key Features
* **Cloud Data Integration:** Connects securely with Azure Cosmos DB to fetch live patient records and clinical/genetic datasets.
* **XGBoost Classification:** Predicts accurate breast cancer subtypes using a trained machine learning model.
* **SHAP Explainability Analysis:** Utilizes SHAP (SHapley Additive exPlanations) values to interpret model predictions and highlight the most impactful/effective genes for specific subtypes.
* **Executive Clinical Summary:** Automatically generates comprehensive AI-driven and clinical summary reports based on prediction probabilities and gene impacts.

## 🛠️ Tech Stack
* **Frontend/UI:** Streamlit, Matplotlib
* **Machine Learning:** XGBoost, Scikit-learn, SHAP
* **Database:** Azure Cosmos DB
* **Data Processing:** Pandas, NumPy

## 📁 Repository Structure
```text
├── container/
│   ├── classifier_xgb_model.pkl
│   ├── encoderf_xgb.pkl
│   └── features_list.pkl
├── app.py
├── analyzer_model.py
├── azure_connection.py
├── fetch_data.py
├── requirements.txt
└── README.md
```
## ⚙️ Local Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/HIMA6768/brest-cancer-subtype-shap-analyzer.git](https://github.com/HIMA6768/brest-cancer-subtype-shap-analyzer.git)
   cd brest-cancer-subtype-shap-analyzer
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
Configure environment variables:
Create a `.env` file in the root directory and add your Azure Cosmos DB credentials:

```env
URL=your_cosmos_db_url
KEY=your_cosmos_db_key
database=your_database_name
container=your_container_name
```
Run the application locally:

```bash
streamlit run app.py
```
📄 **License:** This project is open-source and available under the MIT License.
   
