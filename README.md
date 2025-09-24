# 🖥️ OS Log Anomaly Detection using Data Analytics & Machine Learning

## 📌 Project Overview
Operating systems generate massive amounts of logs that capture events such as system activity, user authentication, and errors.  
Manually analyzing these logs is time-consuming and error-prone.  

This project builds a **Data Analytics + Machine Learning pipeline** to:
- Parse and clean OS logs
- Extract meaningful patterns
- Detect anomalies (suspicious activities, unusual errors)
- Visualize results in a user-friendly way

By combining **Operating System knowledge** with **Data Science + Cybersecurity**, this project creates a practical **Intrusion Detection + System Reliability** tool.

---

## 🎯 Objectives
- Learn **50% of Data Analytics & ML concepts** through a real-world project.  
- Automate **log parsing, feature extraction, and anomaly detection**.  
- Provide **real-time insights** into system health and security.  
- Gain **industry-relevant experience** useful in placements.  

---

## 🔑 Key Features
- 📂 **Log Collection**: Works with Linux syslogs, authentication logs (`auth.log`), or public datasets.  
- 🧹 **Data Preprocessing**: Regex parsing, cleaning, and structuring raw logs into CSV/JSON.  
- 📊 **Analytics**: Error frequency, peak times, suspicious login attempts.  
- 🤖 **ML Models**: Unsupervised anomaly detection (Isolation Forest, One-Class SVM).  
- 📈 **Visualization**: Interactive dashboards with real-time anomaly alerts.  
- 🔐 **Security Use-Case**: Detect brute-force login attempts and intrusion patterns.  

---

## ✨ What Makes This Project Unique?
Instead of repeating generic log analysis projects, this implementation adds **placement-focused uniqueness**:

1. **OS-Specific Focus**  
   - Specialized in **Linux Authentication Logs (`auth.log`)**.  
   - Detects suspicious logins, failed SSH attempts, and brute-force attacks.  

2. **Domain Integration (OS + Cybersecurity)**  
   - Goes beyond system reliability → doubles as a **lightweight intrusion detection system**.  
   - Aligns with **real-world cybersecurity monitoring** used in enterprises.  

3. **Hybrid Approach**  
   - Mix of **rule-based detection** (e.g., >10 failed logins in a minute 🚨) and **ML-based anomaly detection**.  
   - Balances **accuracy + explainability**, making it practical for companies.  

4. **Deep Learning for Log Sequences**  
   - Experimental use of **LSTMs/Transformers** to model **log event sequences**.  
   - Helps detect anomalies not just by frequency, but also by unusual **patterns of events**.  

5. **Visualization Layer**  
   - Real-time **Streamlit dashboard** for monitoring.  
   - Shows spikes in errors, failed login maps, and ML-detected anomalies.  

---

## 🛠️ Tech Stack
- **Programming**: Python 3.8+  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Regex, NLTK  
- **Deep Learning** (optional): TensorFlow / PyTorch for LSTM/Transformers  
- **Visualization**: Streamlit (dashboard)  
- **OS Logs**: `/var/log/auth.log`, `/var/log/syslog` (Linux) or Event Viewer (Windows)  

---

## 📂 Dataset
- **Option A**: Use your system logs (`/var/log/` on Linux).  
- **Option B**: Public datasets from [LogHub](https://github.com/logpai/loghub) (e.g., HDFS, BGL).  

---

## 📖 Project Workflow
### 🔹 Phase 1: Log Collection & Parsing
- Collect logs from OS or dataset.  
- Use regex to extract **timestamp, process, log level, message**.  

### 🔹 Phase 2: Data Analytics
- Perform EDA (error counts, login attempt analysis).  
- Plot unusual spikes and trends.  

### 🔹 Phase 3: Machine Learning
- Feature engineering: Convert logs into structured features.  
- Train ML models for anomaly detection:  
  - Isolation Forest  
  - One-Class SVM  
  - LSTM/Transformer (for advanced sequence learning)  

### 🔹 Phase 4: Hybrid Detection
- Combine **rules + ML models** for more robust anomaly detection.  

### 🔹 Phase 5: Visualization & Insights
- Build a **Streamlit dashboard**.  
- Show anomalies, error spikes, failed login patterns.  

---

## 📊 Example Log Entry
Raw log:
Sep 24 10:15:42 ubuntu sshd[1234]: Failed password for invalid user root from 192.168.1.10 port 22 ssh2

Structured CSV:
| Timestamp           | Host   | Process | PID  | Message                                      |
|---------------------|--------|---------|------|----------------------------------------------|
| 2025-09-24 10:15:42 | ubuntu | sshd    | 1234 | Failed password for invalid user root...     |

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/os-log-anomaly-detection.git
cd os-log-anomaly-detection
2. Install Requirements
pip install -r requirements.txt

3. Run Preprocessing Script
python parse_logs.py

4. Train ML Model
python anomaly_detection.py

5. Launch Dashboard (Optional)
streamlit run dashboard.py
```
---
📌 Future Improvements

Real-time monitoring & alerting (Slack/Email notifications).

Support for cloud logs (AWS CloudWatch, Azure Monitor, GCP Stackdriver).

Integration with SIEM tools for enterprise-scale security.
---

📈 Learning Outcomes

OS fundamentals (logs, processes, authentication events).

Data Analytics (EDA, visualization).

ML for anomaly detection (classical + deep learning).

Rule-based + ML hybrid system design.

Cybersecurity + AI integration.

---

🏢 Industry Relevance

This project is highly relevant in roles like:

Data Analyst (log analytics, EDA).

Machine Learning Engineer (anomaly detection).

Cybersecurity Analyst (intrusion detection).

DevOps / SRE (system monitoring & automation).
---
👨‍💻 Author
Namitha R– Computer Science & Engineering Student

Passionate about AI/ML, Data Analytics, Cybersecurity, and Real-world Applications

