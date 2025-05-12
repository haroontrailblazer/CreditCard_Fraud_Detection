# Project Name

## 🚀 Overview
Project Name is a [short description – e.g., lightweight web app, ML model, data visualization tool] built using [tech stack] to [core functionality or goal]. It is designed for [target audience or use case].

## 🧰 Tech Stack
- Python 3.11
- [Frameworks/Libraries, e.g., Flask, TensorFlow, React, etc.]
- [Database, if applicable]
- [Other tools, e.g., Docker, GitHub Actions]


## ⚙️ Steps

### 1. Load and Examine Data

- Read CSV using pandas
- Display dataset info, check for missing values
- Show class distribution

### 2. Split Data

- Stratified split to ensure fraud presence in all sets
- Final splits:
  - Train: 170,883 samples
  - Validation: 56,961 samples
  - Test: 56,963 samples (100 fraud cases)

### 3. Visualize Data

- Class distribution
- Boxplot of Amount by class
- Histograms of Time and principal components (V1-V5)

### 4. Preprocessing

- Standard scaling applied to `Time` and `Amount`
- Manual undersampling:
  - Balanced training set (294 fraud, 294 normal)

### 5. Summary Statistics

Displays full details of data shapes, class counts after all steps.

## 📉 Class Imbalance Handling

Class distribution (original):
- Normal: 284,315
- Fraud: 492 (~0.17%)

After manual undersampling:
- Normal: 294
- Fraud: 294

## 📎 Notes

- Ensure the dataset is downloaded locally before running.
- Use `StandardScaler` only on training data and apply to validation/test.

## 🔗 Resources

- [Kaggle Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- [sklearn documentation](https://scikit-learn.org/stable/)

---

## 🧪 Future Improvements

- Try SMOTE or ADASYN instead of undersampling
- Experiment with various ML models (RandomForest, XGBoost, etc.)
- Use precision-recall curve and AUC for evaluation

---

## 🧑‍💻 Author

Harshineeshree - Data Analyst | ML Engineer | AI Enthusiast

---



# Install dependencies
pip install -r requirements.txt

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/project-name.git
cd project-name

# (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
