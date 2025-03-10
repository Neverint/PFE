## **PFE - Strengthening Linux Security with Machine Learning and SIEM**

### **Project Description**

As part of this end-of-studies project, our goal is to enhance Linux system security by combining Machine Learning approaches with a SIEM (Security Information and Event Management) system. The main objective is to detect and prevent cyberattacks by leveraging artificial intelligence models capable of identifying malicious behavior in system and network logs.

### **Objectives**
1. **Data Collection and Preprocessing**: Extracting and preparing data from system logs, authentication logs, and network traffic logs to train Machine Learning models.
2. **Development of a Machine Learning Model**: Implementing algorithms capable of detecting both known and unknown threats through supervised, unsupervised, and semi-supervised approaches.
3. **Integration with SIEM**: Deploying the model within a SIEM (Splunk, ELK, QRadar) to analyze logs in real-time and generate alerts.
4. **Implementation of an Alerting and Visualization System**: Configuring dashboards and alerts to help security teams monitor incidents and respond quickly.

### **Technologies and Tools Used**
- **Operating Systems**: Linux (Ubuntu, Debian, CentOS)
- **Machine Learning**: Scikit-Learn, TensorFlow, PyTorch
- **Log Management**: Splunk, ELK Stack (Elasticsearch, Logstash, Kibana), QRadar
- **Development**: Python (Pandas, NumPy, Flask, FastAPI)
- **Automation and Deployment**: Docker, Kubernetes, Ansible

### **Why This Project?**
With the rise of cyberattacks, it is crucial to improve threat detection on Linux systems. Traditional SIEM solutions, while powerful, can generate a large number of false positives. By integrating Machine Learning, we can enhance detection accuracy, reduce unnecessary alerts, and proactively strengthen cybersecurity.

This project represents a step toward smarter and more autonomous security, combining the power of SIEM with the predictive capabilities of Machine Learning.



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
