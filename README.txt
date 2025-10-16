# Autism Screening Classification using Machine Learning

A machine learning project for autism screening in toddlers using the Q-CHAT-10 (Quantitative Checklist for Autism in Toddlers) questionnaire data.

## Project Overview

This project implements and compares traditional machine learning models for autism spectrum disorder (ASD) screening in toddlers aged 12-36 months.
The models achieve exceptional performance (97-100% accuracy) on the Q-CHAT-10 dataset.

## Dataset

- **Primary Dataset**: Toddler Autism dataset July 2018 (1,054 cases)
- **Source**: [https://www.kaggle.com/datasets/fabdelja/autism-screening-for-toddlers/data?select=Toddler+Autism+dataset+July+2018.csv]
- **Features**: 
  - 10 Q-CHAT-10 questionnaire responses (A1-A10)
  - Demographics (Age, Sex, Ethnicity)
  - Family history (Jaundice, Family member with ASD)
  - Respondent information

**Note**: The `Qchat-10-Score` feature is excluded to prevent overfitting, as recommended by dataset authors.

## Key Results

| Model | F1 Score | Accuracy |
|-------|----------|----------|
| Logistic Regression | 1.0000 | 100.0% |
| SVM (RBF) | 1.0000 | 100.0% |
| XGBoost | 0.9954 | 99.4% |
| Random Forest | 0.9767 | 96.9% |

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/autism-screening-ml.git
cd autism-screening-ml

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Requirements
pandas>=1.5.0
numpy>=1.23.0
scikit-learn>=1.2.0
xgboost>=1.7.0
imbalanced-learn>=0.10.0
matplotlib>=3.6.0
seaborn>=0.12.0
jupyter>=1.0.0tebook.ipynb
```

## Disclaimer

This project is for research and educational purposes only. It is not intended for clinical diagnosis. Always consult qualified healthcare professionals for autism screening and diagnosis.

## Acknowledgments

- Q-CHAT-10 questionnaire developers
- Dr Fadi Thabtah for Dataset contribution
