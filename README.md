# Hotel Booking Cancellation Prediction using Logistic Regression

## Project Overview
This project builds a **binary classification model** using **Logistic Regression** to predict whether a hotel booking will be **Cancelled (1)** or **Not Cancelled (0)**, based on customer and booking attributes.

## Dataset
- **Name:** Hotel Reservations Dataset
- **Source:** https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset
- **Rows:** ~36,275 | **Columns:** 19
- **Target Variable:** `booking_status` (Canceled / Not_Canceled)

## Project Structure
```
├── Hotel_Cancellation_Prediction.ipynb   # Main Jupyter Notebook (executed)
├── Hotel Reservations.csv                # Dataset
├── README.md                             # Project documentation
└── requirements.txt                      # Required Python libraries
```

## How to Run the Code

### Step 1: Clone the Repository
```bash
git clone https://github.com/manojsithrama/hotel-cancellation-prediction
cd hotel-cancellation-prediction
```

### Step 2: Install Required Libraries
```bash
pip install -r requirements.txt
```

### Step 3: Add the Dataset
Place `Hotel Reservations.csv` in the same folder as the notebook.

### Step 4: Run the Notebook
```bash
jupyter notebook Hotel_Cancellation_Prediction.ipynb
```
Then click **Kernel → Restart & Run All**.

## Methodology
1. Load and explore the dataset
2. Drop Booking_ID, encode target variable
3. One-hot encode categorical features
4. Split into 70% train / 30% test
5. Build full logistic regression model (statsmodels)
6. Select significant features (p-value ≤ 0.05)
7. Rebuild final model and predict on test set
8. Evaluate with Confusion Matrix, Accuracy, ROC-AUC, Feature Coefficients

## Evaluation Metrics
- Confusion Matrix
- Accuracy Score
- Precision, Recall, F1-Score
- ROC-AUC Score
- Feature Coefficient Chart

## Requirements
See `requirements.txt`
