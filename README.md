<h1 align="center">🧠 Predicting Blockchain Transaction Types using ML Models</h1>

<p align="center">A machine learning project to classify blockchain transactions into sales, purchases, transfers, scams, and phishing attempts.</p>

---

## 📋 Project Overview
This project explores the application of various machine learning models to predict transaction types within blockchain data. The dataset was sourced from Kaggle and contained ~78,600 records. The primary goal is to improve fraud detection in blockchain transactions using effective classification techniques.

## 🚀 Features
✅ Implemented multiple ML models for classification:<br>
 &bull; Random Forest<br>
 &bull; K-Nearest Neighbors (KNN)<br>
 &bull; Gaussian Naive Bayes<br>
 &bull; Decision Tree<br>
 &bull; AdaBoost<br>
✅ Applied effective preprocessing techniques like:
 &bull; Oversampling, Undersampling, Stratified Learning, and SMOTE<br>
 &bull; Information Gain for feature selection<br>
 &bull; Min-Max Normalization for feature scaling<br>
✅ Evaluated model performance using metrics like accuracy, precision, recall, and F1-score.

## 🗄️ Dataset
- **Source:** Kaggle Blockchain Dataset
- **Size:** ~78,600 records
- **Attributes:** Various transaction details, including timestamps, regions, and behavioral patterns.

**Data Imbalance Challenge:** The dataset had a skewed distribution with legitimate transactions heavily outnumbering fraudulent ones. Techniques such as oversampling, undersampling, and SMOTE were implemented to mitigate this issue.

## 🔍 Data Preprocessing
- **Dropped Irrelevant Features:** Removed attributes like `timestamp`, `sending_address`, and `receiving_address`.
- **Handling Missing Values:** Used median imputation for numerical values.
- **Categorical Encoding:** Applied Label Encoding to variables such as `location_region`, `purchase_pattern`, `age_group`, and `anomaly`.
- **Feature Scaling:** Used Min-Max Normalization to ensure consistent feature scaling.

## ⚙️ Models & Hyperparameter Tuning
| Model                | Key Hyperparameters         | Best Accuracy |
|---------------------|-----------------------------|----------------|
| **AdaBoost**          | `n_estimators`, `learning_rate` | 72.9%          |
| **Gaussian Naive Bayes** | `var_smoothing`            | 69.2%          |
| **KNN**               | `n_neighbors`, `weights`       | 97.8%          |
| **Random Forest**     | `n_estimators`, `min_samples_split` | 97.9%      |

✅ Best-performing Model: **Random Forest Classifier**

## 📊 Results & Analysis
- **Random Forest** achieved the highest accuracy of **97.9%** and demonstrated consistent performance across various configurations.
- **KNN** closely followed with an accuracy of **97.8%**, excelling particularly in 'purchase' and 'sale' transactions.
- The **AdaBoost** and **Gaussian Naive Bayes** models struggled with certain transaction types, such as 'phishing' and 'scam'.

## 🔮 Future Improvements
📈 Exploring additional ensemble models like XGBoost and Gradient Boosting.<br>
🧹 Investigating advanced preprocessing techniques for better feature extraction.<br>
🧠 Improving model performance for minority class predictions through enhanced sampling techniques.<br>

## 🤝 Contributors
- **Omnia Osama Ahmed**  
- **Sara Imad Hamdan**  
- **Nour Bashar Soukieh**

## 📄 Course Work
This project was developed for the course Artificial Intelligence (CSC406) In Abu Dhabi Uniersity.

---
<p align="center">💻 Built with ❤️ for secure digital transactions in the Metaverse!</p>
