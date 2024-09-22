# Random Forest and GBDT - DonorsChoose Dataset

This project applies **Random Forest (RF)** and **Gradient Boosting Decision Trees (GBDT)** to predict the approval of project proposals on DonorsChoose.org. The assignment focuses on feature engineering, hyperparameter tuning, and model evaluation using AUC scores.

## Dataset
- **DonorsChoose.org project proposals**.
- **Features**: Project titles, essays, resource summaries, teacher and school metadata.
- **Target**: Binary classification for project approval (1: approved, 0: not approved).

## Key Features
- **Text Processing**: Applied TF-IDF and Bag of Words (BOW) techniques to project essays and titles.
- **Categorical Features**: Response encoding for features like school state, grade category, and teacher prefix.
- **Numerical Features**: Processed features such as resource prices and project quantities.

## Models Implemented
1. **Random Forest**:
   - Used response encoding and text vectorization (BOW, TF-IDF) to train the model.
   - Hyperparameter tuning for `n_estimators` and `max_depth`.

2. **GBDT**:
   - Applied GBDT using the same feature sets, with similar hyperparameter tuning.

## Results
- **Best AUC Score**: Achieved high AUC scores using optimized hyperparameters for both RF and GBDT models.
- **Performance Evaluation**: Plotted ROC curves and heatmaps to visualize model performance across different parameter values.

## Conclusion
Both Random Forest and GBDT performed well in predicting project approvals, with GBDT slightly outperforming Random Forest in AUC score. Hyperparameter tuning played a significant role in maximizing model performance.
