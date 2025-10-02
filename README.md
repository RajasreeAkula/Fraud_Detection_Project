# FraudDetection_Project

Real-world financial fraud detection simulation analyzing transactions, detecting anomalies, and visualizing flagged patterns

**Project Overview**

This project simulates a real-world financial fraud detection scenario for a credit card provider. The objective was to detect unusual or fraudulent transactions using a hybrid workflow of Excel, SQL, Python (ML), and Power BI, reflecting how financial institutions integrate data engineering, machine learning, and business intelligence for fraud risk monitoring.

**Tools & Technologies**

Excel – Initial cleaning, derived features, pivot analysis

SQL (MySQL) – Transactional queries, business insights, fraud indicators

Python (Scikit-learn) – Preprocessing, anomaly detection (Isolation Forest)

Power BI – Interactive dashboards for fraud reporting

Visualization – Matplotlib, Seaborn, Power BI visuals

**Project Workflow**

1. Excel – Data Foundation
   
Cleaned and preprocessed dataset

Derived features: log-transformed transaction amount, transaction time (hour, day, month), days since last transaction

Pivot tables & charts for early EDA

2. Python ML – Anomaly Detection
   
Preprocessed data (scaling, encoding categorical variables)

Applied Isolation Forest (contamination = 0.05)

Created Anomaly_Flag (1 = Fraud, 0 = Normal) and anomaly scores

Detected ~6% anomalies (~30/503 samples flagged)

3. SQL – Business Insights

Total transactions analyzed: 2,512

Key findings:

Debit usage > Credit usage

ATM transactions had the highest average value

Fort Worth = busiest location; Portland = anomaly hotspot

Doctors held higher account balances; Students generated most revenue

High login attempts strongly correlated with high transaction amounts

4. Power BI – Fraud Monitoring Dashboard

Designed interactive dashboard with KPIs:

Total transactions, Total Amount, Distinct Accounts, % Flagged Txns

Visuals included:

Transaction volume by channel & location

Occupation-wise spending and balances

Flagged transaction trends by date & time (heatmap + summary tables)

High-value anomaly tracking

Enabled real-time monitoring & decision-making view

**Key Insights**

Students contributed the highest transaction volume, while Doctors held the largest balances

Fort Worth emerged as the busiest transaction hub; Portland had suspicious high-value anomalies

ATM transactions had the highest average values → potential fraud risk zone

High login attempts + high transaction amounts flagged as strong fraud indicators

**Learning Outcomes**

Built a full end-to-end fraud detection pipeline

Applied unsupervised anomaly detection (Isolation Forest) in real data

Generated business-driven insights via SQL & visualization

Project Team 1.Aastha 2.Aditya Bajantri 3.Rajasri 4.Aman Singh

Integrated Excel, SQL, Python, and Power BI into a single fraud analytics workflow

Improved ability to explain fraud detection findings to both technical and business stakeholders

Project Team 1.Aastha 2.Aditya Bajantri 3. Akula Rajasree 4.Aman Singh
