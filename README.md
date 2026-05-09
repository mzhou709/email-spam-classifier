# Email Spam Classifier

Email spam classifier using TF-IDF, feature engineering, and logistic regression with cross-validation on the [SpamAssassin public corpus](https://spamassassin.apache.org/old/publiccorpus/) - 99.3% accuracy, 97.3% 
recall, and zero false positives. 

## Results

| Model | Accuracy | Recall | F1 | AUC |
|---|---|---|---|---|
| Baseline LR (word indicators) | 90.5% | 72.5% | 80.3% | 0.939 |
| Naive Bayes (TF-IDF) | 97.5% | 93.7% | 95.2% | 0.997 |
| Logistic Regression (TF-IDF) | 99.3% | 97.3% | 98.6% | 0.9998 |

## Project Workflow

```
Train/Val Split + EDA
    ↓
Text Preprocessing
    ↓
Feature Engineering (TF-IDF + Structural Features)
    ↓
Baseline Model (Word Indicators + Logistic Regression)
    ↓
Hyperparameter Tuning (5-fold CV)
    ↓
Validation Set Evaluation
```
