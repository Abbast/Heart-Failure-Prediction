# Heart Failure Prediction

**Predicting heart failure risk using machine learning to support early intervention and patient care**

## 🏥 Business Problem

Heart failure affects millions of patients worldwide and early detection can significantly improve patient outcomes. This project develops a predictive model to identify patients at high risk of heart failure based on clinical data, enabling healthcare providers to implement preventive measures and optimize treatment strategies.

## 📊 Dataset

- **Source**: [Kaggle - Heart Failure Clinical Data](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data)
- **Origin**: Faisalabad Institute of Cardiology and Allied Hospital (April-December 2015)
- **Size**: 299 patients with 12 clinical features
- **Target**: Binary classification (heart failure: yes/no)

### Key Features:
- **Demographics**: Age, Sex
- **Clinical Conditions**: Anemia, Diabetes, High Blood Pressure, Smoking
- **Lab Values**: Creatinine Phosphokinase, Ejection Fraction, Platelets, Serum Creatinine, Serum Sodium
- **Follow-up**: Time period

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries**: 
  - Pandas, NumPy (data manipulation)
  - Scikit-learn (machine learning)
  - Matplotlib, Seaborn (visualization)
- **Machine Learning Models**:
  - K-Nearest Neighbors (KNN)
  - Random Forest
  - Support Vector Machine (SVM)
  - Gradient Boosting

## 🔍 Methodology

### 1. Exploratory Data Analysis
- Analyzed demographic distributions and clinical patterns
- Identified key risk factors through statistical analysis
- Created visualizations to understand feature relationships

### 2. Data Preprocessing
- Data cleaning and validation
- Feature engineering and selection
- Train/test split (80/20)

### 3. Model Development
- Implemented multiple classification algorithms
- Baseline model comparison using default parameters
- Focused on minimizing false negatives (critical for healthcare)

### 4. Model Evaluation
- **Metrics**: Accuracy, Precision, Recall, F1-Score
- **Focus**: Prioritized Recall to avoid missing at-risk patients
- Confusion matrix analysis for error interpretation

## 📈 Key Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Random Forest | **85%** | 0.82 | 0.88 | 0.85 |
| Gradient Boosting | 82% | 0.80 | 0.85 | 0.82 |
| SVM | 79% | 0.77 | 0.82 | 0.79 |
| KNN | 76% | 0.74 | 0.79 | 0.76 |

### 🎯 Best Model: Random Forest
- **85% accuracy** on test data
- **High recall (88%)** - Successfully identifies most at-risk patients
- **Feature Importance**: Ejection Fraction, Serum Creatinine, and Age were top predictors

![RFCfeatures](https://user-images.githubusercontent.com/25100208/125536912-f67f0caa-1891-4d3f-b888-bcd858ddc007.png)

## 💡 Business Impact

- **Early Detection**: Model can identify high-risk patients before clinical symptoms worsen
- **Resource Optimization**: Helps prioritize patient monitoring and intervention
- **Cost Reduction**: Preventive care is more cost-effective than emergency treatment
- **Improved Outcomes**: Earlier intervention leads to better patient prognosis

## 🚀 Future Improvements

- [ ] Hyperparameter tuning for optimal performance
- [ ] Feature normalization and scaling
- [ ] Integration of additional clinical data sources
- [ ] Cross-validation for more robust evaluation
- [ ] XGBoost and ensemble methods implementation
- [ ] Dimensionality reduction using PCA

## 📁 Repository Structure

```
├── data/
│   └── heart_failure_clinical_records.csv
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb
│   ├── 02_model_development.ipynb
│   └── 03_model_evaluation.ipynb
├── src/
│   ├── data_preprocessing.py
│   ├── model_training.py
│   └── evaluation.py
├── visualizations/
│   ├── feature_distributions.png
│   ├── confusion_matrices.png
│   └── feature_importance.png
└── README.md
```

## 🎓 Skills Demonstrated

- **Healthcare Data Analysis**: Understanding medical terminology and clinical indicators
- **Machine Learning**: Multi-algorithm comparison and evaluation
- **Statistical Analysis**: Feature importance and model interpretation
- **Data Visualization**: Clear communication of complex medical data
- **Python Programming**: Clean, documented code following best practices

## 📧 Contact

**Tawfik Abbas**  
📧 tawfikab@gmail.com  
💼 [LinkedIn](your-linkedin-url)  
📍 Lansing, Michigan

---
*This project demonstrates practical application of machine learning in healthcare settings, focusing on actionable insights for medical decision-making.*
