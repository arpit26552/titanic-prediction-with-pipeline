# Decision Tree Prediction Pipeline

This project implements a complete machine learning pipeline using a **Decision Tree Classifier** with `scikit-learn`. The pipeline includes all preprocessing steps (like encoding and missing value handling) and is saved as a `.pkl` file (`pipe.pkl`) for easy reuse and deployment.

---

## 🚀 Features

- Built using `scikit-learn`'s `Pipeline` object
- Fully automated:
  - Missing value handling
  - One-hot encoding / label encoding
  - Decision Tree Classifier training
- Exported pipeline using `pickle`

---
## 🔧 How to Use

### Step 1: Load the pipeline

```python
import pickle

# Load the pipeline
with open('pipe.pkl', 'rb') as f:
    pipe = pickle.load(f)

# Make predictions
preds = pipe.predict(X_new)
