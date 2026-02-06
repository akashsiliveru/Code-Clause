<p align="center">
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
</p>

<h1 align="center"> Credit Card Fraud Detection System</h1>

<p align="center">
<b>Machine Learning • Anomaly Detection • Imbalanced Data</b>
</p>

<p align="center">
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
</p>

## Model Performance — What I Observed

<p align="center">
  <img src="https://media.giphy.com/media/hgjNPEmAmpCMM/giphy.gif" width="350">
</p>

While working on this project, I focused on detecting fraudulent transactions using **unsupervised anomaly detection models** because the dataset is extremely imbalanced.

Out of more than **2,84,807 transactions**, only **492 were fraud** — which makes this a challenging real-world problem.

---

## Models I Tried

<p align="center">
  <img src="https://img.shields.io/badge/Isolation%20Forest-Anomaly%20Detection-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Local%20Outlier%20Factor-Density%20Based-green?style=for-the-badge">
</p>

I experimented with:

- **Isolation Forest** — detects anomalies using random trees  
- **Local Outlier Factor (LOF)** — detects points with low local density  

## How I Evaluated the Models

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=22&duration=3000&color=F75C7E&center=true&vCenter=true&width=600&lines=Precision+%7C+Recall+%7C+F1-Score;Accuracy+alone+is+misleading+here" />
</p>

Since this is a fraud detection problem, I didn’t rely only on accuracy.  
I paid more attention to:

- Precision  
- Recall  
- F1-score  

because missing fraud cases is more costly than false alarms.

##  Results I Got

### 🔹 Isolation Forest

| Metric | Score |
|--------|-------|
| Accuracy | **99.74%** |
| Fraud Precision | **0.26** |
| Fraud Recall | **0.27** |
| Fraud F1-Score | **0.26** |
| Total Errors | **73** |

This model was able to detect a reasonable number of fraud cases compared to LOF.

### Local Outlier Factor (LOF)

| Metric | Score |
|--------|-------|
| Accuracy | **99.65%** |
| Fraud Precision | **0.02** |
| Fraud Recall | **0.02** |
| Fraud F1-Score | **0.02** |
| Total Errors | **97** |

LOF struggled to identify fraud cases because the dataset is extremely imbalanced.

##  What I Learned From This

<p align="center">
  <img src="https://media.giphy.com/media/iPj5oRtJzQGxwzuCKV/giphy.gif" width="400">
</p>

- High accuracy does not mean good fraud detection  
- Isolation Forest performs better for anomaly-based fraud detection  
- Evaluation metrics matter more than the algorithm itself  
- Real-world ML problems are rarely balanced  

---

##  Skills I Demonstrated

✔ Handling imbalanced datasets  
✔ Applying anomaly detection algorithms  
✔ Interpreting fraud detection metrics  
✔ Understanding trade-offs between false positives and false negatives  
