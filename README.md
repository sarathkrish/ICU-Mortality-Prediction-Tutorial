# ICU Mortality Prediction Tutorial

## 🎯 Overview
This tutorial teaches how to build a machine learning model for predicting ICU mortality using MIMIC-III data. You'll learn feature engineering from electronic health records, Random Forest classification, and clinical evaluation metrics.

## 📋 Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or VS Code with Python extension
- Basic knowledge of Python and pandas

## 🚀 Setup Instructions

### Step 1: Clone/Download This Repository
```bash
git clone [your-repository-url]
cd ICU-Mortality-Prediction-Tutorial
```

### Step 2: Download MIMIC-III Demo Dataset
1. **Visit**: https://physionet.org/content/mimiciii-demo/1.4/
2. **Download** the complete dataset (mimic-iii-clinical-database-demo-1.4.zip)
3. **Extract** the zip file to the project root directory
4. **Verify** the folder structure looks like this:
```
ICU-Mortality-Prediction-Tutorial/
├── mimic-iii-clinical-database-demo-1.4/
│   ├── PATIENTS.csv
│   ├── ADMISSIONS.csv
│   ├── ICUSTAYS.csv
│   └── [other MIMIC files...]
├── tutorial/
├── requirements.txt
└── README.md
```

### Step 3: Create Virtual Environment (Recommended)
```bash
# Create virtual environment
python -m venv tutorial_env

# Activate virtual environment
# On macOS/Linux:
source tutorial_env/bin/activate
# On Windows:
tutorial_env\Scripts\activate
```

### Step 4: Install Required Packages
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Step 5: Launch Jupyter Notebook
```bash
# Navigate to tutorial folder
cd tutorial/notebooks

# Start Jupyter
jupyter notebook

# Open: icu_mortality_ml.ipynb
```

## 📊 Tutorial Contents

### What You'll Learn:
- ✅ Load and explore MIMIC-III clinical database
- ✅ Engineer features from electronic health records
- ✅ Build Random Forest classifier for mortality prediction  
- ✅ Evaluate model performance using clinical metrics
- ✅ Interpret feature importance for healthcare insights

### Expected Results:
- **AUC Score**: ~0.62 (moderate discrimination)
- **Key Predictors**: ICU length of stay, admission type, insurance
- **Clinical Insights**: Actionable findings for healthcare providers

## 🔧 Troubleshooting

### Common Issues:

**Dataset Path Error:**
- Ensure MIMIC dataset is in the correct location
- Check that folder name matches: `mimic-iii-clinical-database-demo-1.4`

**Missing Packages:**
```bash
# If packages fail to install, try:
pip install --upgrade setuptools wheel
pip install -r requirements.txt
```

**Jupyter Kernel Issues:**
```bash
# Install ipykernel in your virtual environment
pip install ipykernel
python -m ipykernel install --user --name=tutorial_env
```

## 📁 Project Structure
```
ICU-Mortality-Prediction-Tutorial/
├── mimic-iii-clinical-database-demo-1.4/    # Download from PhysioNet
│   ├── PATIENTS.csv
│   ├── ADMISSIONS.csv  
│   ├── ICUSTAYS.csv
│   └── [other files...]
├── tutorial/
│   └── notebooks/
│       └── icu_mortality_ml.ipynb           # Main tutorial
├── requirements.txt                         # Python dependencies
└── README.md                               # This file
```

## 🎓 Learning Objectives
By completing this tutorial, you will understand:
1. Healthcare data preprocessing and feature engineering
2. Random Forest classification for clinical prediction
3. Proper evaluation metrics for healthcare ML
4. Feature importance interpretation in medical context
5. Best practices for reproducible healthcare ML research

## 📚 Additional Resources
- **MIMIC-III Documentation**: https://mimic.mit.edu/docs/iii/
- **PhysioNet**: https://physionet.org/
- **Scikit-learn Documentation**: https://scikit-learn.org/

## ⚠️ Important Notes
- This tutorial uses the MIMIC-III **demo dataset** (publicly available)
- For full MIMIC-III access, you need to complete PhysioNet credentialing
- Results are for educational purposes only
- Always follow ethical guidelines when working with healthcare data

---
**🏥 Remember**: Machine learning in healthcare should augment, not replace, clinical judgment!
