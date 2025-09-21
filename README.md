# Predicting Heart Disease Using Machine Learning

A comparative study of Logistic Regression, Random Forest, and XGBoost for heart disease prediction, highlighting the critical challenge of class imbalance in medical datasets.

## 📖 Abstract

Cardiovascular diseases (CVDs) are the leading cause of death globally. This research applies machine learning to predict heart disease status using a dataset of 10,000 subjects. We compared three models: Logistic Regression, Random Forest, and XGBoost. While the Random Forest model achieved high accuracy (79.95%), detailed analysis revealed a critical class imbalance issue, underscoring a key challenge in using real-world medical data for predictive modeling. Feature importance analysis confirmed the clinical relevance of factors like age, cholesterol level, and blood pressure.

## 📊 Key Findings

-   **Model Performance:** Random Forest achieved the highest accuracy (79.95%) but failed to identify any true positive cases (precision = 0, recall = 0), indicating severe bias toward the majority class.
-   **Primary Challenge:** The dataset exhibits significant class imbalance, which is a major obstacle for building effective predictive models in healthcare.
-   **Clinical Relevance:** Feature importance analysis correctly identified age, cholesterol level, and blood pressure as top predictors, aligning with established medical knowledge.
-   **Main Takeaway:** This project demonstrates that high accuracy can be misleading and emphasizes the necessity of using comprehensive metrics (precision, recall, F1) and techniques to handle imbalance in medical ML.

## 🗂️ Project Structure
Heart_Disease/
│
├── heart_disease_analysis.ipynb # Main Jupyter Notebook with full code
├── heart_disease.csv # Dataset (get it from Kaggle link below)
├── Bristi_Heart_Disease_ML_Report.pdf # Complete research paper
└── README.md # This file

text

## ⚙️ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/farjana-bristy/Heart_Disease.git
    cd Heart_Disease
    ```

2.  **Install required Python libraries:**
    ```bash
    pip install pandas numpy scikit-learn xgboost matplotlib seaborn imbalanced-learn
    ```

3.  **Download the Dataset:**
    The dataset is sourced from Kaggle. Download it from the link below and place the `heart_disease.csv` file in the project directory.
    *   [Heart Disease Dataset on Kaggle](https://www.kaggle.com/datasets/oktayrdeki/heart-disease)

## 🚀 Usage

Open and run the Jupyter Notebook `heart_disease_analysis.ipynb` cell-by-cell to:
1.  Load and explore the data.
2.  Preprocess the data (handle missing values, scaling, encoding).
3.  Address class imbalance using SMOTE.
4.  Train and evaluate the three machine learning models.
5.  Generate performance metrics and visualizations.

## 📈 Results Summary

| Model                | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
| :------------------- | :------: | :-------: | :----: | :------: | :-----: |
| Logistic Regression  |  0.5090  |   0.190   | 0.445  |  0.266   |  0.476  |
| **Random Forest**    | **0.7995**|  **0.000**|**0.000**| **0.000**| **0.523**|
| XGBoost              |  0.6685  |   0.192   | 0.205  |  0.198   |  0.504  |

## 🔍 reproducibility

All results are reproducible thanks to fixed random seeds (`RANDOM_SEED = 42`). The complete methodology, including data preprocessing, feature engineering, and model training, is thoroughly documented in the accompanying research paper.

## 📄 Research Paper

The full research paper, providing detailed context, methodology, discussion, and conclusions, is available here:
[`heart_disease_research_bristi.pdf`](heart_disease_research_bristi.pdf)

This paper has also been archived on Zenodo for long-term access and citation:
[![DOI](https://zenodo.org/badge/DOI/https://doi.org/10.5281/zenodo.17169393.svg)](https://doi.org/10.5281/zenodo.17169393)

## 👩‍💻 Author

**Khadeja Farjana Bristi** - Independent Researcher
-   Email: fbristy44@gmail.com
-   LinkedIn: [linkedin.com/in/farjana-bristy](https://www.linkedin.com/in/farjana-bristy/)
-   GitHub: [github.com/farjana-bristy](https://github.com/farjana-bristy)

## 🙏 Acknowledgments

-   Dataset provided by [Oktay Rdeki](https://www.kaggle.com/oktayrdeki) on Kaggle.
-   Libraries: Pandas, Scikit-learn, XGBoost, Matplotlib, Seaborn, Imbalanced-learn.

## 📜 License  

© 2025 Khadeja Farjana Bristi. This work is licensed under a [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
