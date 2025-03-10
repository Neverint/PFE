# PFE - Project de fin d'étude 


### **Phase 1: Data Collection and Preprocessing**
**Goal:** Gather and preprocess cybersecurity data for training the ML model.

#### **Step 1: Gather Cybersecurity Datasets**
You need a dataset containing network traffic logs, authentication logs, system events, and labeled/unlabeled attack data. Some great sources:
- [CICIDS 2017](https://www.unb.ca/cic/datasets/ids.html) (Intrusion Detection System logs)
- [NSL-KDD](https://www.kaggle.com/datasets/siddharthapalani/nsl-kdd-dataset) (Network Intrusion Dataset)
- [UNSW-NB15](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/) (Cyber attack dataset)
- [MITRE ATT&CK Framework](https://attack.mitre.org/)

#### **Step 2: Data Preprocessing**
- Convert raw logs into structured formats (e.g., CSV, JSON).
- Handle missing values, normalize data, and remove duplicates.
- Feature Engineering: Extract relevant features from raw logs (e.g., request frequency, source IP, login attempts).
- Label Encoding: If working with labeled data, ensure labels are formatted for ML training.

Would you like me to help preprocess a dataset if you have one?

---

### **Phase 2: Machine Learning Model Development**
**Goal:** Build an ML model capable of detecting both known and unknown cyber threats.

#### **Step 3: Choose the Right ML Approach**
You should consider:
- **Supervised Learning (for labeled datasets)** – Use models like Random Forest, XGBoost, or Deep Learning.
- **Unsupervised Learning (for anomaly detection on unknown attacks)** – Use Isolation Forest, Autoencoders, or One-Class SVM.
- **Semi-Supervised Learning** – Mix both for better generalization.

#### **Step 4: Model Training**
- Train the model in Python using **Scikit-Learn**, **TensorFlow**, or **PyTorch**.
- Evaluate the model using Precision, Recall, F1-Score, and AUC-ROC.

Do you have a preference for a specific ML technique?

---

### **Phase 3: SIEM Integration**
**Goal:** Deploy the ML model in a SIEM system like Splunk, ELK, or QRadar.

#### **Step 5: Deploy Model in SIEM**
- Convert the trained model into an API (Flask or FastAPI).
- Configure SIEM to send logs to the model for analysis.
- Return detected anomalies as alerts to SIEM.

Would you like help in setting up the API?

---

### **Phase 4: Real-Time Alerting & Dashboard**
**Goal:** Notify security teams and visualize cyber threats.

#### **Step 6: Implement Alerts**
- Configure the SIEM to trigger alerts for high-risk threats.
- Send alerts via email, Slack, or a ticketing system.

#### **Step 7: Build Dashboards**
- Use **Splunk**, **Grafana**, or **Kibana** to visualize detected attacks.
- Display attack patterns, severity levels, and sources.
