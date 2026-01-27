# soc_home_lab
this is my soc analyst roadmap and training
# 🛡️ SOC Analyst Portfolio (Splunk • Sysmon • Detection Labs)

**Author:** Srihari Nalluri
**Role Target:** SOC Analyst (L1 → L2)
**Focus:** SIEM • Incident Detection • Log Analysis • Blue Team Operations

---

## 📌 About This Repository

This repository contains **hands-on SOC (Security Operations Center) projects** built using **Splunk**, **Sysmon**, and real-world attack simulations.

The goal of this portfolio is to demonstrate:

* Practical SIEM skills (Splunk SPL, dashboards, alerts)
* Endpoint and network log analysis
* Detection engineering fundamentals
* Incident investigation and documentation
* SOC analyst thinking (false positive vs true positive)

All labs are performed in a **controlled home SOC environment** for learning and defensive purposes.

---

## 🧠 Skills Demonstrated

* SIEM Operations (Splunk Enterprise)
* Windows Event Log Analysis
* Sysmon Endpoint Telemetry
* SPL Query Writing
* Brute Force Detection
* Network Scan Detection (Nmap)
* Malware Behavior Analysis
* MITRE ATT&CK Mapping
* Incident Documentation
* SOC Alert Lifecycle

---

## 🏗️ Lab Environment

| Component        | Description                             |
| ---------------- | --------------------------------------- |
| OS               | Windows 10/11                           |
| SIEM             | Splunk Enterprise (Free)                |
| Endpoint Logging | Sysmon (SwiftOnSecurity config)         |
| Log Forwarding   | Splunk Universal Forwarder / Winlogbeat |
| Attack Tools     | Nmap, Windows native tools              |

---

## 📂 Repository Structure

```text
soc-home-lab/
│
├── 00-environment-setup/
│   ├── splunk-installation.md
│   ├── sysmon-installation.md
│   └── log-forwarding-setup.md
│
├── 01-splunk-basics/
│   ├── splunk-fundamentals.md
│   ├── basic-spl-queries.md
│   └── dashboards.md
│
├── 02-brute-force-detection/
│   ├── attack-simulation.md
│   ├── detection-logic.md
│   ├── spl-queries.md
│   ├── screenshots/
│   └── incident-report.md
│
├── 03-network-scan-detection/
│   ├── nmap-attack.md
│   ├── detection-logic.md
│   ├── spl-queries.md
│   ├── mitre-mapping.md
│   └── incident-report.md
│
├── 04-malware-behavior-detection/
│   ├── attack-simulation.md
│   ├── process-analysis.md
│   ├── spl-queries.md
│   ├── persistence-analysis.md
│   └── incident-report.md
│
├── 05-phishing-investigation/
│   ├── email-analysis.md
│   ├── header-analysis.md
│   ├── ioc-extraction.md
│   └── investigation-report.md
│
├── 06-dashboards-and-alerts/
│   ├── security-dashboards.md
│   ├── alert-rules.md
│   └── tuning-and-false-positives.md
│
└── README.md
```

---

## 🔍 Featured Projects

### 🔹 Project 1: SOC Home Lab Setup

**Objective:** Build a functional SOC lab with endpoint telemetry and SIEM ingestion.

**Highlights:**

* Installed and configured Splunk Enterprise
* Deployed Sysmon for deep endpoint visibility
* Forwarded logs into Splunk
* Validated log ingestion and parsing

---

### 🔹 Project 2: Brute Force Detection

**Objective:** Detect repeated authentication failures indicating a brute force attack.

**Data Sources:**

* Windows Security logs (Event ID 4625)

**Detection Logic:**

* Multiple failed logins from same source
* Time-based threshold detection

**MITRE ATT&CK:**

* T1110 – Brute Force

---

### 🔹 Project 3: Network Scan Detection (Nmap)

**Objective:** Identify internal network reconnaissance activity.

**Data Sources:**

* Sysmon Event ID 3 (Network Connections)

**Detection Logic:**

* Multiple destination ports accessed in short time

**MITRE ATT&CK:**

* T1046 – Network Service Discovery

---

### 🔹 Project 4: Malware Behavior Detection

**Objective:** Detect suspicious process execution and persistence mechanisms.

**Indicators:**

* Encoded PowerShell
* Suspicious parent-child processes
* Registry persistence

**MITRE ATT&CK:**

* T1059 – Command and Scripting Interpreter
* T1547 – Boot or Logon Autostart Execution

---

### 🔹 Project 5: Phishing Investigation

**Objective:** Analyze phishing emails and extract indicators of compromise.

**Steps:**

* Email header analysis
* Sender validation
* URL and hash analysis

**MITRE ATT&CK:**

* T1566 – Phishing

---

## 📊 Dashboards & Alerts

* Authentication Failure Monitoring
* Network Activity Overview
* Suspicious Process Execution
* Malware Indicators Dashboard

Alerts are tuned to reduce false positives and follow SOC escalation best practices.

---

## 🎯 How This Maps to SOC Roles

| SOC Skill              | Demonstrated |
| ---------------------- | ------------ |
| Alert Triage           | ✅            |
| Log Analysis           | ✅            |
| Detection Engineering  | ✅            |
| Incident Documentation | ✅            |
| MITRE Mapping          | ✅            |
| SIEM Usage             | ✅            |

---

## 🧪 How to Reproduce These Labs

Each project folder contains:

* Step-by-step attack simulation
* Detection queries
* Screenshots
* Incident report

Follow the **00-environment-setup** folder to build the same lab.

---

## 📌 Disclaimer

All activities in this repository were performed in a **controlled lab environment** for educational and defensive purposes only.

---

## 📫 Contact

* **LinkedIn:** [https://www.linkedin.com/](https://www.linkedin.com/)
* **Email:** [sriharinalluri25@gmail.com](mailto:sriharinalluri25@gmail.com)

---

⭐ *This repository is designed to reflect real-world SOC analyst responsibilities and is actively maintained as skills progress.*
