# 💳 Credit Card Fraud Detection

## 📌 About
A machine learning classification project that detects fraudulent credit card transactions from a highly imbalanced dataset of **284,807 transactions**. Used **under-sampling** technique to handle class imbalance and trained a Logistic Regression model achieving **93.9% accuracy**.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn

## 📊 Dataset
- **Total Transactions:** 284,807
- **Legitimate Transactions:** 284,315 (99.83%)
- **Fraudulent Transactions:** 492 (0.17%)
- **Features:** 30 (V1-V28 from PCA transformation + Time + Amount)
- **Target:** Class (0 = Legitimate, 1 = Fraud)

## 🔍 What I Did

### 1. Data Exploration
- Analyzed distribution of legitimate vs fraudulent transactions
- Found extreme class imbalance (99.83% vs 0.17%)
- Compared statistical measures (mean Amount) for both classes
- Verified no missing values in the dataset

### 2. Handling Class Imbalance — Under-Sampling
- Randomly sampled **492 legitimate transactions** to match the 492 fraud cases
- Created a balanced dataset of **984 total records** (50/50 split)
- This prevents the model from being biased toward the majority class

### 3. Model Training
- Split data: 80% training (787 records) / 20% testing (197 records)
- Used **stratified split** to maintain class balance in both sets
- Trained a **Logistic Regression** classifier

### 4. Results
| Metric | Score |
|--------|-------|
| Training Accuracy | **94.15%** |
| Testing Accuracy | **93.91%** |

## 🏆 Key Takeaways
- Under-sampling effectively balanced the highly skewed dataset
- Logistic Regression performed well with minimal overfitting (training ≈ testing accuracy)
- The model can correctly identify ~94% of fraudulent transactions

## 📂 Project Structure
```
├── credit_data.csv                       # Dataset
├── Credit_Card_Fraud_Detection.ipynb     # Jupyter Notebook
└── README.md                             # Project Documentation
```

## 🚀 How to Run
1. Clone this repository
   ```bash
   git clone https://github.com/chiragsddsdc/credit-card-fraud-detection.git
   ```
2. Install dependencies
   ```bash
   pip install pandas numpy scikit-learn
   ```
3. Open the notebook
   ```bash
   jupyter notebook Credit_Card_Fraud_Detection.ipynb
   ```

## 📬 Contact
- **Email:** chiragyadav2424@gmail.com
