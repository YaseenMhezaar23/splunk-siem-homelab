🛡️ Splunk SIEM Homelab – SOC Monitoring Project
📌 Overview

This project demonstrates a hands-on Splunk SIEM homelab built to simulate real-world SOC (Security Operations Center) monitoring and log analysis scenarios.

The lab focuses on:

Log ingestion

Threat detection

Alert creation

Dashboard visualization

Basic incident investigation

🎯 Objectives

Understand how SIEM works in a SOC environment

Practice log analysis and correlation

Detect suspicious activities using Splunk SPL

Create SOC dashboards and alerts

🧰 Tools & Technologies Used

Splunk Enterprise

Linux (Ubuntu/Kali)

Sample Logs (Apache, Auth, Windows Events)

SPL (Search Processing Language)

🏗️ Lab Architecture

Log sources send data to Splunk

Splunk parses and indexes logs

Searches, dashboards, and alerts are created for monitoring

📷 Architecture Diagram:


📥 Log Sources Ingested

Web server access logs (Apache)

Authentication logs

Simulated Windows security events

🔍 Use Cases Implemented

Failed login detection

Brute-force attack simulation

HTTP error analysis

Suspicious IP activity tracking

🚨 Alerts Created

Multiple failed login attempts from a single IP

Suspicious access to admin pages

Repeated authentication failures

Alert logic and SPL queries are available in the alerts/ folder.

📊 Dashboards

Login success vs failure

Top source IPs

HTTP status codes

Event volume over time

📷 Dashboard screenshots:


🧪 Sample SPL Queries
index=web_logs status=403 OR status=401
| stats count by src_ip


More queries are available in the queries/ folder.

🚀 Key Learnings

Hands-on SIEM experience

Understanding SOC workflows

Writing efficient SPL queries

Building alerts and dashboards

Incident analysis mindset

📌 Future Improvements

Integrate Wazuh

Add real-time alerts

Simulate malware logs

Map detections to MITRE ATT&CK

🔗 LinkedIn Post

You can find the LinkedIn showcase post here:
https://www.linkedin.com/posts/yaseen-mhezaar_splunk-siem-homelab-activity-7403335019148034048-xpuL?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAFMLY5wBaTSh4tPtil-XLDZfIhdXbV5Lsu0

🧑‍💻 Author

Yaseen Mhezaar
Aspiring SOC Analyst | Cybersecurity Enthusiast
