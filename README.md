# VaultMind

![Gradio-Based User Interface](https://github.com/user-attachments/assets/4bd3b766-7041-499b-87c8-fefcaa3dfd20)

VaultMind is a machine learning-powered tool designed to predict bankruptcy in SMEs using financial data. It combines high accuracy with interpretability through a Gradio-based interface.

This repository provides a bankruptcy prediction tool for Small and Medium Enterprises (SMEs), aiming to provide interpretable results through a user-friendly interface. The ensemble model outperforms traditional methods, achieving high reliability in financial distress prediction.

## 🔍 Core Features:

* **Ensemble Model**: Combines Logistic Regression, Random Forest, and XGBoost (Voting Classifier) achieving **96.63% accuracy** and **99.6% ROC AUC**.
* **Explainability**: Uses **SHAP (SHapley Additive exPlanations)** to highlight key financial ratios influencing predictions.
* **Narrative Reports**: Generates human-readable summaries using **Natural Language Generation (NLG)**.

![Bankruptcy Prediction Report](https://github.com/user-attachments/assets/6f0a4eb8-c020-482d-94b6-c0b1ea5908cb)

## ⚙️ Workflow:

1. **Data Preparation**:

   * Dataset of 427 companies with 66 financial features.
   * Preprocessing steps: missing value imputation, outlier detection, normalization, and SMOTE for class balancing.

2. **Model Development**:

   * Built using Logistic Regression, Random Forest, and XGBoost.
   * Combined via Voting Classifier.
   * Evaluated with accuracy, ROC AUC, and F1-scores.
   * Final performance: **96.63% accuracy**, **99.6% ROC AUC**.

3. **User Interface and Interpretability**:

   * Developed using Gradio for seamless interaction.
   * Users can input financial metrics and get real-time predictions.
   * SHAP integration for interpretable visual explanations.

4. **Automated Report Generation**:

   * Utilizes NLG to create detailed, readable reports.
   * Includes predictions, influential features, and financial recommendations.

![Workflow Diagram](https://github.com/user-attachments/assets/159e6ccb-d02b-4dd5-a853-2e32072f27c8)

## 🚀 Getting Started

### Prerequisites

* Python 3.12
* Install required libraries listed in `requirements.txt`

### Running the Project

1. **Model Training**:

   * Execute `ModelTraining.ipynb` to preprocess data and train models.
2. **Launching the Interface**:

   * Run `GradioApp.py` to launch the Gradio UI locally.
   * Click the generated link to interact via browser.

## ✅ Results

* High-performing ensemble model with excellent generalization.
* SHAP analysis ensures transparency and builds user trust.
* Generated reports help users understand results and guide decision-making.

## 🔹 Conclusion

VaultMind offers a robust, interpretable solution for predicting bankruptcy risk in SMEs. By merging machine learning accuracy with visual and textual interpretability, it serves as a valuable tool for financial analysts, decision-makers, and business stakeholders.
