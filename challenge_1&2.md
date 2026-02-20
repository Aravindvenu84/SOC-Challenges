# 🛡️ CyberDefenders Challenge Report  
## WebStrike & QRadar101 Investigation Case Study

---

# 🔎 Challenge 1: WebStrike

---

## i) Challenge Overview & Objectives

**Platform:** CyberDefenders  
**Challenge Name:** WebStrike  
**Focus Area:** Network Traffic Analysis / Web Attack Investigation  

### Objective:

The objective of the WebStrike challenge was to:

- Analyze captured network traffic.
- Identify malicious activity within HTTP communications.
- Detect web-based attacks.
- Extract indicators of compromise (IOCs).
- Determine attacker behavior and impact.

---

## ii) Step-by-Step Methodology

### 1️⃣ Traffic Capture Analysis

- Opened the provided `.pcap` file in **Wireshark**.
- Applied filters such as:
  - `http`
  - `tcp`
  - Suspicious IP filtering
- Identified abnormal HTTP requests.

---

### 2️⃣ Suspicious Activity Identification

- Reviewed:
  - GET and POST requests
  - Unusual parameters
  - Suspicious payloads in HTTP traffic
- Checked for:
  - SQL injection patterns
  - Command injection attempts
  - Web shell uploads

---

### 3️⃣ IOC Extraction

- Identified:
  - Malicious IP addresses
  - Suspicious URLs
  - Indicators within HTTP payloads
- Followed TCP streams to reconstruct attacker activity.

---

### 4️⃣ Attack Confirmation

- Correlated abnormal requests with responses.
- Confirmed malicious exploitation attempts.
- Determined attack vector and potential impact.

---

## iii) Screenshots

> 📸  following screenshots in this section:
- Wireshark traffic overview
- HTTP filtered traffic
- Follow TCP Stream output
- Identified malicious payload

(Example format)

![Wireshark Overview](screenshots/webstrike_overview.png)
![HTTP Analysis](screenshots/webstrike_http.png)

---

## iv) Key Findings, Challenges & Resolution

### Key Findings

- Malicious HTTP requests detected.
- Suspicious payload patterns in web parameters.
- Clear evidence of web-based exploitation attempt.
- Identified attacker IP address.

### Challenges Faced

- None significant.
- The challenge was straightforward and completed quickly.

### Resolution

- Block malicious IP.
- Strengthen web application filtering.
- Implement WAF rules to detect injection patterns.

---

# 🧠 Challenge 2: QRadar101

---

## i) Challenge Overview & Objectives

**Platform:** CyberDefenders  
**Challenge Name:** QRadar101  
**Focus Area:** SIEM Investigation / Log Correlation  

### Objective:

The objective of the QRadar101 challenge was to:

- Investigate alerts using IBM QRadar SIEM.
- Analyze offense details.
- Correlate logs.
- Identify attacker activity and scope.
- Determine root cause and impact.

---

## ii) Step-by-Step Methodology

### 1️⃣ Offense Review

- Logged into the QRadar interface.
- Reviewed the generated offense.
- Checked:
  - Magnitude
  - Categories
  - Source & Destination IPs

---

### 2️⃣ Log Correlation

- Investigated events contributing to the offense.
- Filtered logs based on:
  - Source IP
  - Username
  - Event type
- Analyzed authentication attempts and suspicious activity.

---

### 3️⃣ Deep Log Analysis

- Examined:
  - Failed and successful logins
  - Network connections
  - Time correlation between events
- Identified suspicious patterns.

---

### 4️⃣ Root Cause Determination

- Correlated multiple events.
- Identified the attacker behavior.
- Determined whether the attack was successful.
- Evaluated impact on the system.

---

## iii) Screenshots

> 📸 Insert the following screenshots:
- QRadar Offense dashboard
- Event log filtering
- Log correlation view
- Final offense summary

![QRadar Offense](screenshots/qradar_offense.png)
![Event Correlation](screenshots/qradar_logs.png)

---

## iv) Key Findings, Challenges & Resolution

### Key Findings

- Successfully identified suspicious activity through log correlation.
- Understood offense magnitude scoring.
- Determined attacker scope and impact.

### Challenges Faced

- QRadar interface was new to me.
- Navigation and filtering required research.
- Understanding event correlation took time.

### Resolution

- Conducted additional research on QRadar functionalities.
- Explored event filtering techniques.
- Completed investigation successfully after deep analysis.

---

# ⚖️ Comparison: WebStrike vs QRadar101

| Aspect | WebStrike | QRadar101 |
|--------|-----------|------------|
| Type | Network Traffic Analysis | SIEM Log Correlation |
| Tool Used | Wireshark | IBM QRadar |
| Difficulty Level | Easy | Moderate to Hard |
| Learning Curve | Minimal | Significant |
| Investigation Depth | Packet-level analysis | Multi-log correlation |

### Key Differences

- WebStrike focused on packet-level network visibility.
- QRadar101 focused on centralized log analysis.
- WebStrike was quick and straightforward.
- QRadar101 required deeper research and SIEM understanding.

---

# 📈 Overall Learning & Skill Enhancement

These challenges significantly improved my SOC investigation skills:

### From WebStrike:
- Improved packet analysis using Wireshark.
- Strengthened understanding of HTTP-based attacks.
- Practiced IOC extraction from network traffic.

### From QRadar101:
- Learned how to navigate and investigate within a SIEM.
- Understood offense correlation and magnitude scoring.
- Improved log analysis and investigation workflow.
- Developed patience and research-based problem-solving skills.

---

# 🏁 Conclusion

Completing both challenges enhanced my practical SOC capabilities:

- Strengthened my ability to analyze raw network traffic.
- Improved SIEM investigation skills.
- Learned to correlate logs and identify attacker behavior.
- Gained hands-on experience with real-world investigation workflows.

While WebStrike tested my technical speed in packet analysis, QRadar101 challenged my analytical depth and adaptability to new SIEM environments.

These practical tasks helped bridge the gap between theoretical cybersecurity knowledge and real SOC investigation experience.
