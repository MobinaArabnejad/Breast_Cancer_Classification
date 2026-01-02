---

## What this project does
- Loads the dataset from CSV
- Performs basic exploratory data analysis (EDA):
  - Class distribution
  - Summary statistics
  - Correlation heatmap
  - Feature distributions/plots
- Cleans the dataset:
  - Removes non-informative columns (e.g., id, unnamed columns)
  - Encodes target label (`M` → 1, B → 0)
- Trains a RandomForestClassifier within a scikit-learn Pipeline
- Uses GridSearchCV (5-fold) to tune hyperparameters
- Evaluates performance on a test split using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (Precision/Recall/F1)
  - ROC Curve + ROC-AUC
- Extracts and visualizes Top feature importances from the trained model

---

## Tech Stack
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## How to run

### 1) Clone the repository
```bash
git clone https://github.com/MobinaArabnejad/breast-cancer-classification.git
cd breast-cancer-classification

''' ## Dataset

This project uses the Breast Cancer Wisconsin dataset.

- Source: Kaggle (UCI ML repository)  
- Link: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data '''
