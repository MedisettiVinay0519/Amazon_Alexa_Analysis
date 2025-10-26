# Amazon Alexa Sentiment Analysis

## 🎯 Project Overview
This project focuses on **Sentiment Analysis** of **Amazon Alexa customer reviews** to classify customer feedback as either positive (1) or negative (0). By applying **Natural Language Processing (NLP)** techniques and various Machine Learning models, the goal was to build a robust classifier that can automatically gauge user satisfaction.

---

## 🛠️ Key Techniques
* **Data Source:** Amazon Alexa customer reviews dataset.
* **NLP Technique:** **Count Vectorizer** for converting text data into a matrix of token counts (feature extraction).
* **Data Preparation:** The dataset was balanced to ensure equal representation of positive and negative feedback before training.

---

## 🧠 Machine Learning Models & Results
To determine the most effective classification approach, the following four models were trained and evaluated using the preprocessed review data.

| Model | Accuracy |
| :--- | :--- |
| **Support Vector Classifier (SVC)** | **0.9568** |
| Logistic Regression | 0.9430 |
| Multinomial Naive Bayes (MNB) | 0.9309 |
| Gradient Boosting Classifier | 0.8808 |

### Best Performing Model
The **Support Vector Classifier (SVC)** yielded the highest performance, achieving an **Accuracy of 0.9568** (**95.68%**). This model was chosen for making predictions, as it demonstrated the strongest generalization capability in classifying customer sentiment.
## 📊 Model Evaluation: Support Vector Classifier (SVC)

The final SVC model was evaluated using a **Confusion Matrix** to thoroughly assess its performance.

| | Predicted Negative (0) | Predicted Positive (1) |
| :--- | :--- | :--- |
| **Actual Negative (0)** | **500** (True Negatives) | **50** (False Positives) |
| **Actual Positive (1)** | **88** (False Negatives) | **520** (True Positives) |

### Confusion Matrix Visualization
![Confusion Matrix for SVC Model on Amazon Alexa Reviews](images/Screenshot%202025-10-26%20115339.png)
