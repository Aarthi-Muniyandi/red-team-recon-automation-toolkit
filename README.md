# Red Team Recon Automation Toolkit

The Red Team Recon Automation Toolkit is an automated reconnaissance framework developed for cybersecurity professionals, penetration testers, and security researchers to streamline the information gathering and attack surface mapping phase of security assessments.

The system integrates multiple reconnaissance techniques into a unified platform, automating target enumeration, service discovery, technology fingerprinting, risk evaluation, and report generation through a centralized web-based dashboard.

The toolkit reduces manual effort, accelerates reconnaissance workflows, and provides structured risk analysis using CVSS-based severity scoring.

# Problem Statement

Reconnaissance is one of the most critical phases in penetration testing and red-team operations. Traditional recon workflows require analysts to use multiple independent tools for:

+ subdomain discovery,
+ host identification,
+ port scanning,
+ directory enumeration,
+ and technology fingerprinting.

This fragmented process increases:

+ operational complexity,
+ execution time,
+ manual correlation effort,
+ and difficulty in prioritizing security risks.

The Red Team Recon Automation Toolkit addresses these challenges by automating and consolidating reconnaissance operations into a single platform.

## Key Features
+ Automated Reconnaissance Workflow
+ End-to-end automated recon execution
+ Unified target scanning pipeline
+ Reduced manual enumeration effort
+ Multiple Scan Modes
**Simple Scan**

Fast reconnaissance for quick attack surface discovery.

**Deep Scan**

Comprehensive enumeration and detailed service analysis.

# Reconnaissance Modules
+ Subdomain Enumeration
+ Live Host Detection
+ Port Scanning
+ Service Detection
+ Directory Enumeration
+ Web Technology Fingerprinting
+ DNS & WHOIS Enumeration
  **CVSS-Based Risk Scoring**
+ Automated risk evaluation
+ Vulnerability severity prioritization
+ Structured attack surface analysis
  **Web Dashboard**
+ Scan management interface
+ Real-time scan visualization
+ Centralized result aggregation
  **Automated Report Generation**
+ HTML report export
+ PDF report generation
+ Structured reconnaissance summaries
  
# System Workflow
Target Input
      ↓
Recon Module Execution
      ↓
Data Aggregation
      ↓
Risk Evaluation (CVSS)
      ↓
Report Generation

# System Architecture
**Core Components**
+ Web Interface (Flask)
+ Recon Engine
+ Data Aggregation Layer
+ Risk Analysis Engine
+ Reporting Module
**Technology Stack**
**Backend**
Python
Flask Framework
**Frontend**
HTML
CSS
JavaScript
**Database**
SQLite
**Integrated Tools & Libraries**
Nmap
Requests
BeautifulSoup
Regex
JSON
WeasyPrint
Python-Nmap
# Recon Modules
| **Module** | **Function** |
| ---------- | ------------ |
| subdomain.py | Subdomain enumeration |
| live_hosts.py	| Active host discovery |
| port_scan.py | Port and service scanning |
| directory_enum.py | Directory brute forcing |
| tech_fingerprint.py	| Web technology detection |
| risk_engine.py | CVSS-based risk scoring |

# Project Structure
red-team-recon-automation-toolkit/
│
├── recon/
├── templates/
├── static/
├── reports/
├── images/
│
├── app.py
├── config.py
├── database.py
├── init_db.py
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore

**Installation**
**Clone Repository**
```
git clone https://github.com/Aarthi-Muniyandi/red-team-recon-automation-toolkit.git
```
Navigate to Project Directory
```
cd red-team-recon-automation-toolkit
```
Create Virtual Environment
```
python -m venv venv
```
Activate Environment
Windows
```
venv\Scripts\activate
```
Linux / macOS
```
source venv/bin/activate
```
Install Dependencies
```
pip install -r requirements.txt
```
Initialize Database
```
python init_db.py
```
Running the Application
```
python app.py
```
Open in browser:
```
http://127.0.0.1:5000
```

# Report Generation

After scan completion, the system generates structured reconnaissance reports containing:

+ discovered assets,
+ open ports,
+ detected services,
+ identified technologies,
+ and calculated risk scores.

Reports can be exported in:

+ HTML format
+ PDF format

# Future Enhancements
+ AI-assisted threat intelligence correlation
+ Parallel scan execution
+ Advanced vulnerability integration
+ Real-time monitoring dashboard
+ Containerized deployment
+ Cloud-based recon orchestration
+ Machine learning-based anomaly detection
  
# Disclaimer

This project is intended strictly for:

+ educational purposes,
+ authorized penetration testing,
+ and cybersecurity research.

Do not use this tool against systems or networks without explicit authorization.

Unauthorized scanning may violate legal and ethical regulations.

# License

Licensed under the MIT License.

# Author

Aarthi M
Cybersecurity Student | Red Teaming Enthusiast
