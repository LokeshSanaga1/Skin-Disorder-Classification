

# Skin Disorder Classification

## Overview
This project aims to improve the diagnosis of **erythemato-squamous diseases (ESDs)** in dermatology by leveraging machine learning to analyze clinical and histopathological features. The system enhances diagnostic accuracy, optimizes biopsy decision-making, reduces misdiagnosis, and minimizes unnecessary treatments, contributing to cost savings and better patient outcomes. It uses a dataset with 34 features (12 clinical, 22 histopathological) and ensures privacy compliance by anonymizing patient data.

### Key Objectives
- Accurate detection of six ESDs: **psoriasis, seborrheic dermatitis, lichen planus, pityriasis rosea, chronic dermatitis, pityriasis rubra pilaris**.
- Early identification using a 0-3 graded scale for clinical features.
- Support medical research and resource optimization in healthcare.

## Domain Analysis
- **Erythemato-squamous diseases (ESDs)**: Common skin conditions causing inflammation and scaling (e.g., psoriasis affects 2-3% of the population).
- Challenges: Overlapping symptoms (erythema, scaling) make differential diagnosis difficult, often requiring biopsies.
- Features: Includes clinical (e.g., itching, family history) and histopathological (e.g., hyperkeratosis, Munro microabscess) attributes.

## Dataset Features
- **Clinical**: Erythema, scaling, itching, Koebner phenomenon, family history, etc.
- **Histopathological**: Acanthosis, parakeratosis, spongiosis, band-like infiltrate, etc.
- Full feature descriptions available in the [project documentation](#).

## Business Case
- Improves diagnostic precision, reducing misdiagnosis and unnecessary biopsies.
- Enhances patient care through early detection and cost-effective treatment.
- Contributes to dermatological research and healthcare efficiency.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/LokeshSanaga1/Skin-Disorder-Classification.git
   cd Skin-Disorder-Classification
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Requirements
```
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
imblearn
```

## Usage
1. **Prepare Data**:
   - Load and preprocess the dataset (e.g., handle missing values, encode labels).
2. **Train Model**:
   - Run the script to train the XGBoost model (best-performing among tested models: Logistic Regression, SVM, KNN, Decision Tree, Random Forest).
   - Example:
     ```bash
     python train_model.py
     ```
3. **Evaluate**:
   - Assess performance using accuracy, precision, recall, F1-score, and ROC-AUC.
4. **Predict**:
   - Use the trained model for new ESD predictions.

## Methodology
- **Data Preprocessing**: Handled imbalanced classes with SMOTE, encoded categorical features.
- **Model Selection**: Tested multiple classifiers; **XGBoost** outperformed others.
- **Evaluation**: Used cross-validation and metrics like accuracy and F1-score.

## Results
- **Best Model**: XGBoost achieved the highest accuracy and reliability for ESD classification.
- Reduces diagnostic errors and supports clinical decision-making.

## Contributing
Feel free to submit issues or pull requests to enhance the project.

