# 💧 Prediction of Water Quality using Machine Learning

This project aims to predict the potability of water (safe or unsafe for drinking) using machine learning techniques.
The model is trained on a dataset of water quality indicators and classifies samples as potable (1) or not potable (0).

## 📂 Dataset

- **Name:** Water Potability Dataset  
- **Source:** [UCI / Kaggle - Water Quality Dataset]  
- **Description:** The dataset includes physicochemical properties of water such as:
  - pH
  - Hardness
  - Solids
  - Chloramines
  - Sulfate
  - Conductivity
  - Organic Carbon
  - Trihalomethanes
  - Turbidity
  - Potability (Label)

## 📊 Libraries Used

- `pandas` – For data loading and manipulation  
- `numpy` – For numerical computations  
- `seaborn` & `matplotlib` – For data visualization  
- `scikit-learn` – For machine learning model, metrics, and hyperparameter tuning  
- `pickle` – For saving the trained model  

## 🔍 Exploratory Data Analysis (EDA)

- Checked for missing values and handled them by dropping rows.
- Boxplots were used to detect outliers in each feature.
- A heatmap of correlation matrix helped in understanding relationships between features.
- Countplot used to show class distribution (Potable vs Non-potable water).

## 🧠 Machine Learning Model

- **Model Used:** K-Nearest Neighbors (KNN)
- **Train-Test Split:** 80% training, 20% testing
- **Hyperparameter Tuning:** GridSearchCV with 5-fold cross-validation  
  - Tuned parameters: `n_neighbors`, `algorithm`, `p` (Minkowski distance)

## ✅ Evaluation Metrics

- Accuracy Score  
- Confusion Matrix  
- Classification Report  
- Precision Score
- Recall Score  
- Silhouette Score

## 📈 Results

- Accuracy:60%
- Best Hyperparameters (via GridSearchCV):
  {'n_neighbors':auto, 'algorithm': '11', 'p':3}

  
