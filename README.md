NETWORK ANOMALY DETECTION PROJECT
FOR TOTAL CODE JUPYTER NOTEBOOK CLICK HERE FOR STREAMLIT APP CODE CLICK HERE

An anomaly detection system for identifying unusual network behavng machine learning algorithms in Python. This project offers an end-to-end approach to network anomaly detection, starting with data exploration and visualization in Tableau, followed by exploratory data analysis (EDA), hypothesis testing, machine learning modeling with experimental tracking, and concluding with deployment.

PROBLEM STATEMENT
In the realm of cybersecurity, network anomaly detection is a critical task that involves identifying unusual patterns or behaviors that deviate from the norm within network traffic. These anomalies could signify a range of security threats, from compromised devices and malware infections to large-scale cyber-attacks like DDoS (Distributed Denial of Service).

As a data scientist working in the cybersecurity department, your task is to visualize and analyze the provided network data (NSL-KDD dataset). Apply supervised learning algorithms to find the best model for classifying the data using the attack column. Utilize unsupervised algorithms to improve the performance and deploy the machine learning models using Streamlit.

TARGET METRIC
Classification metrics such as accuracy, precision, recall, and F1-score were used. However, recall and accuracy were prioritized for network anomaly detection due to their importance in identifying anomalies effectively.

CONTENTS AVAILABLE IN NETWORK_ANOMALY_DETECTION_PROJECT
Definitions & Problem Statement: Detailed feature definitions, dataset origin, and the problem statement.
Tableau Visualization:
Network Connection Metrics Dashboard (Basic and Content-Related Features)
Advanced Traffic Patterns Dashboard (Time and Host-Related Features)
Exploratory Data Analysis Using Python: Data cleaning, feature engineering, and univariate, bivariate, and multivariate data visualizations.
Hypothesis Testing: Conducted between important features and binary/multi-class targets, verifying assumptions and applying non-parametric tests when necessary.
Feature Engineering Using Unsupervised Algorithms: Added features using anomaly detection algorithms and KMeans clustering to enhance classification performance.
Machine Learning Modeling for Binary Classification: Applied and tuned 10 different classification models using MLflow for experimental tracking.
Evaluation of Results for Binary Classification: Plotted and compared metrics of all 10 models.
Multi-Class Classification Utilizing Optimal Models: Applied optimal models after preprocessing and compared their results.
Deployment of the Optimal Model Using Streamlit: Deployed locally and on Streamlit Cloud for real-time predictions.
Conclusion, Actionable Insights, Recommendations, Future Scope & References: Summarized findings and provided relevant links.
FINAL SCORES ACHIEVED
BINARY CLASS CLASSIFICATION
Model: Tuned Adaboost on Balanced Dataset
Parameters: {'algorithm': 'SAMME', 'learning_rate': 0.8065, 'n_estimators': 114}
Training Time: 98.13 seconds
Testing Time: 2.87 seconds
Tuning Time: 227.52 seconds
Train Metrics:

Accuracy: 1.0000
Precision: 1.0000
Recall: 1.0000
F1-score: 1.0000
F2-score: 1.0000
ROC-AUC: 1.0000
PR-AUC: 1.0000
Test Metrics:

Accuracy: 0.9992
Precision: 0.9996
Recall: 0.9988
F1-score: 0.9992
F2-score: 0.9990
ROC-AUC: 1.0000
PR-AUC: 1.0000
MULTI-CLASS CLASSIFICATION
Model: Tuned_Light_GBM_on_Balanced_Dataset
Parameters: {'bagging_fraction': np.float64(0.7809345096873808), 'bagging_freq': 9, 'boosting_type': 'gbdt', 'colsample_bytree': np.float64(1.3021969807540397), 'feature_fraction': np.float64(0.5745506436797708), 'learning_rate': np.float64(0.3060660809801552), 'max_depth': 10, 'min_child_samples': 10, 'min_child_weight': np.float64(0.020871568153417244), 'min_data_in_leaf': 82, 'min_split_gain': np.float64(0.08154614284548342), 'n_estimators': 180, 'num_leaves': 52, 'objective': 'binary', 'random_state': 42, 'reg_alpha': np.float64(0.03702232586704518), 'reg_lambda': np.float64(1.0376985928164089), 'scale_pos_weight': np.float64(0.7317381190502594), 'subsample': np.float64(1.3631034258755936)}
Training Time: 5.65 seconds
Testing Time: 1.84 seconds
Tuning Time: 167.39 seconds
Train Metrics:

Accuracy: 1.0000
Precision (macro): 1.0000
Recall (macro): 1.0000
F1-score (macro): 1.0000
F2-score (macro): 1.0000
Test Metrics:

Accuracy: 0.9990
Precision (macro): 0.9447
Recall (macro): 0.9761
F1-score (macro): 0.9590
F2-score (macro): 0.9689
IMPORTANT LINKS
Network Anomaly Detection Project - GitHub
LinkedIn Profile (Amaanuddin)
Tableau Dashboards
Data Science Portfolio
Project Video Presentation
Project Medium Blog
Streamlit app link (App may go to sleep)
# 🚨 From Network Traffic to Cyber Threat Detection: My Network Anomaly Detection System Project

I’m excited to share one of my recent **Data Science & Machine Learning projects — Network Anomaly Detection System**.

Cybersecurity is becoming increasingly data-driven, and one of the most interesting applications of Machine Learning is identifying network behavior that deviates from normal patterns.

In this project, I worked on building an end-to-end **Machine Learning-based Network Anomaly Detection System** capable of identifying whether network traffic is **NORMAL or an ATTACK**, while also classifying different categories of attacks.

🔹 **The Problem**

Traditional security systems often depend on predefined rules or known indicators of compromise.

Anomaly-based detection takes a different approach: instead of looking only for known threats, it learns patterns of normal behavior and identifies activity that deviates from those patterns.

The objective of this project was to:

✅ Analyze and visualize network traffic
✅ Perform EDA and hypothesis testing
✅ Apply supervised learning for attack classification
✅ Apply unsupervised learning for anomaly detection and feature engineering
✅ Identify the best-performing models
✅ Deploy the final solution for prediction and real-time monitoring

The complete project was structured into four major blocks:

📊 Tableau Visualizations
🔍 EDA & Hypothesis Testing
🤖 Machine Learning Modeling
🚀 Deployment

The project uses the **NSL-KDD dataset**, derived from the KDD-1999 intrusion detection dataset. The attacks are broadly categorized into **DoS, Probe, R2L, and U2R**, along with normal network traffic.

---

### 🔍 1. Exploratory Data Analysis

I started by understanding the structure and behavior of network traffic data, investigating numerical and categorical variables and identifying the characteristics associated with anomalous traffic.

Feature analysis was particularly important because network traffic contains a mixture of continuous, categorical and binary attributes.

Some of the important features identified during the project included:

• `service`
• `srcbytes`
• `dstbytes`
• `diffsrvcount`
• `Flag_SF`
• `error_flag_or_not`
• `urgent_or_not`

These features showed significant importance in the final anomaly detection process.

---

### 🧠 2. Unsupervised Learning for Anomaly Detection

One of the most interesting parts of this project was using **unsupervised learning as a feature-engineering layer** before classification.

I experimented with multiple anomaly-detection and clustering techniques, including:

🔹 Local Outlier Factor (LOF)
🔹 Isolation Forest
🔹 Robust Covariance
🔹 One-Class SVM
🔹 KNN-based distance features
🔹 Gaussian Mixture Model (GMM)
🔹 DBSCAN
🔹 K-Means

The outputs from these models were transformed into additional features that could provide the supervised classifiers with more information about whether a network record behaved like an anomaly.

For example, the pipeline generated features such as:

`binary_lof_nof`
`binary_iforest_df`
`binary_robust_cov_df`
`binary_one_class_svm_df`
`binary_dbscan_labels`
`binary_knn_kth_distance`
`binary_gmm_score`
`binary_kmeans_adv`

This hybrid approach — **unsupervised anomaly detection + supervised classification** — was one of the key technical aspects of the project.

---

### 🤖 3. Supervised Machine Learning

After feature engineering, I developed models for two major prediction tasks:

**Binary Classification**

➡️ NORMAL
➡️ ATTACK

**Multi-Class Classification**

➡️ NORMAL
➡️ DOS
➡️ Probe
➡️ R2L
➡️ U2R

After comparing different models, the project identified:

🏆 **AdaBoost** → Best-performing model for Binary Classification

🏆 **LightGBM** → Best-performing model for Multi-Class Classification

The final model selection was based on performance considerations including **accuracy and latency**.

---

### 📈 4. Model Performance

The final project achieved approximately **99% accuracy on the provided dataset** according to the project report.

This demonstrated that the combination of feature engineering, anomaly-based features and supervised classification could effectively distinguish normal network traffic from malicious activity.

At the same time, I learned an important practical lesson:

**High accuracy alone is not enough in a real-world ML system.**

For cybersecurity applications, we also need to consider:

• False positives and false negatives
• Detection latency
• Feature availability
• Model interpretability
• Scalability
• Ability to detect evolving attack patterns

---

### ⚙️ 5. Feature Engineering & Optimization

A particularly interesting finding was the computational cost introduced by some of the unsupervised algorithms.

For example, **LOF and DBSCAN-based feature engineering took approximately 60 seconds** to generate the associated features.

This highlighted an important production ML trade-off:

> Better feature engineering does not always mean better production performance.

Reducing unnecessary computational overhead could significantly improve inference latency in a real-time monitoring environment.

---

### 🚀 6. Deployment

I also took the project beyond model training by building a **Streamlit-based prediction interface**.

The application accepts network connection characteristics and uses the trained preprocessing pipeline and ML models to generate predictions.

The binary prediction pipeline ultimately returns:

🟢 **NORMAL**

or

🔴 **ATTACK**

The multi-class pipeline can additionally decode the predicted attack category.
This made the project more than just a notebook experiment — it became an end-to-end workflow covering:

**Data → EDA → Feature Engineering → Anomaly Detection → Classification → Model Evaluation → Deployment**

---

### 🛠️ Tech Stack

**Languages & Libraries**

🐍 Python
📊 Pandas
🔢 NumPy
📈 Matplotlib
📊 Seaborn
🤖 Scikit-learn
⚡ LightGBM
📉 Statsmodels

**Machine Learning**

• Supervised Learning
• Unsupervised Learning
• Classification
• Clustering
• Outlier Detection
• Feature Engineering
• Hyperparameter Tuning

**MLOps / Deployment**

• MLflow
• Streamlit
• Pickle/Gzip model serialization

**Visualization**

• Tableau
• Python Visualization

---

### 💡 Key Learnings

This project helped me understand that solving a real-world ML problem is much more than simply training a model.

My major takeaways were:

🔹 **Feature engineering can significantly influence model performance.**

🔹 **Unsupervised learning can be valuable even when the final objective is supervised classification.**

🔹 **Model accuracy must be considered together with latency and computational complexity.**

🔹 **Categorical variables such as `service` and `protocoltype` can have a significant impact on detection performance.**

🔹 **Deployment is an essential part of converting an ML experiment into a usable solution.**

🔹 **Cybersecurity models need continuous adaptation because attack patterns evolve over time.**

---

### 🔮 Future Improvements

There are several directions in which I would like to take this project further:

🚀 Scale the system for real-time, high-volume network traffic

☁️ Explore cloud-based deployment

🔄 Continuously retrain models using updated attack patterns

🌲 Experiment with Random Forest and XGBoost

🧠 Explore Deep Learning approaches such as Autoencoders and RNNs

⚡ Optimize computationally expensive anomaly-detection features

🔐 Integrate the model with existing network monitoring / IDS infrastructure

These directions are also aligned with the project's proposed future scope.

---

### 🎯 Final Takeaway

This project gave me hands-on experience across the complete Data Science lifecycle:

**Business Problem → Data Understanding → EDA → Hypothesis Testing → Feature Engineering → Unsupervised Learning → Supervised Learning → Model Evaluation → Deployment**

More importantly, it strengthened my understanding of how **Machine Learning can be applied to cybersecurity problems**, where the goal is not just prediction, but faster identification of potentially malicious behavior.

I’m looking forward to applying these learnings to more real-world **Data Science, Machine Learning, and AI projects.** 🚀

#DataScience #MachineLearning #CyberSecurity #NetworkSecurity #AnomalyDetection #IntrusionDetection #Python #ScikitLearn #LightGBM #AdaBoost #UnsupervisedLearning #SupervisedLearning #FeatureEngineering #MLflow #Streamlit #Tableau #DataAnalytics #AI #NSLKDD #MachineLearningProjects
