# 🛡️ Credit Card Fraud Detection Model & Handling Imbalanced Data

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine_Learning-orange.svg?logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-Gradient_Boosting-green.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Processing-150458.svg?logo=pandas&logoColor=white)
![Imbalanced-Learn](https://img.shields.io/badge/SMOTE-Data_Balancing-yellow.svg)

## 📌 What is this Project?
Credit card fraud detection is the process of identifying stolen or unauthorized transactions within a massive stream of legitimate purchases. The primary challenge in this domain is **severe class imbalance**—legitimate transactions outnumber fraudulent ones by massive margins (often 99% to 1%). 

This project is an end-to-end Machine Learning pipeline designed to tackle this exact problem. It utilizes data preprocessing, synthetic minority over-sampling (SMOTE), and a comparative analysis of multiple algorithms to evaluate how different models behave when hunting for hidden anomalies in financial data.

### The Data Challenge
The initial dataset contained an extreme class imbalance, which causes standard AI models to fail.

![Original Imbalance](images/imbalance_graph.png)
![Average Transaction Amounts](images/imbalance_data_graph.png)

---

## 🛠️ Tech Stack & Tools Used
* **Programming Language:** Python
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning & Modeling:** Scikit-Learn, XGBoost
* **Data Balancing:** Imbalanced-Learn (SMOTE)
### Applying SMOTE (Synthetic Minority Over-sampling Technique)
To allow the algorithms to learn the fraud patterns, the data was perfectly balanced by synthetically generating minority class examples.

![SMOTE Balanced Data](images/balance_data_graph.png)
* **Model Serialization:** Joblib
---

## 🧠 Machine Learning Models Evaluated
To deeply analyze the dataset, I deployed and compared a diverse set of machine learning algorithms, ranging from basic linear equations to advanced tree-based ensembles:

1. **Logistic Regression:** A baseline linear model used to establish a foundational performance metric.
2. **Decision Tree Classifier:** A non-linear algorithm that splits data based on feature conditions.
3. **Random Forest Classifier:** A powerful bagging ensemble method that utilizes multiple decision trees to reduce overfitting.
4. **Extra Trees Classifier:** An extremely randomized tree ensemble that introduces further randomness to improve generalizability.
5. **XGBoost Classifier:** An advanced gradient boosting framework engineered for maximum computational speed and high performance on complex patterns.

---

## 📊 Evaluation Criteria & Model Judgment
In fraud detection, standard "Accuracy" is a deceptive metric. A model that blindly guesses every transaction is "normal" would still score 99% accuracy, but it would miss 100% of the fraud. 

Therefore, the models in this project were judged based on a strict balance of the following metrics:
* **Recall (Sensitivity):** The percentage of actual fraud successfully caught by the model. *(Crucial for stopping financial loss).*
* **Precision:** The percentage of flagged transactions that were actually fraudulent. *(Crucial for ensuring innocent customers do not get their cards falsely frozen).*
* **F1-Score:** The harmonic mean of Precision and Recall, providing a single, unified score for imbalanced data.

### Comparative Analysis: Check Which Model Works Best
Rather than forcing a single "champion" model, this project presents a side-by-side dashboard of all algorithms trained on both unbalanced and SMOTE-balanced data. This allows observers to objectively compare the trade-offs:
* How linear models (Logistic Regression) struggle with precision after SMOTE.
* How boosting models (XGBoost) require balanced data to uncover complex boundaries.
* How ensemble bagging (Random Forest / Extra Trees) handles synthetic data without massive overfitting.

### Final Model Performance (Balanced Data)

![Model Performance Comparison](images/balanced_data_model_output_graph.png)

---

## 💡 Conclusion
Handling highly imbalanced data requires a delicate intersection of data engineering and algorithm selection. This project successfully demonstrates that balancing the dataset using SMOTE dramatically alters the learning behavior of artificial intelligence. By building a dynamic comparison pipeline, we can observe exactly how different mathematical approaches prioritize catching fraud versus preventing false alarms, ultimately allowing a business to select the exact algorithm that fits their current risk tolerance.

---

---

## 📬 Let's Connect!
I enjoy discussing Data Science, Machine Learning, and innovative tech projects. Whether you have a question about this model, some feedback, or just want to connect, feel free to reach out!

<br>

**Subhadip Biswas**

[![Email](https://img.shields.io/badge/Email-subhadip2622%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:subhadip2622@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Subhadip-cloudCoder)

<br>

<p align="center">
  <b>⭐️ If you found this project helpful or interesting, please consider giving it a star! ⭐️</b>
</p>
