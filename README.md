# Cybersecurity-Team-Lab
📘 Overview
This report summarizes the defensive actions taken during a simulated Blue Team exercise for Sierra College's Cybersecurity Challenge. Our objective was to secure a vulnerable network, detect and respond to attacks, and recommend long-term security improvements.

🧪 Environment Issues Identified: 
- Misconfigured firewall rules (pfSense)
- Default credentials and weak passwords
- Excessive open ports (SSH, RDP, SMTP, etc.)
- No MFA on user/admin accounts

🔐 Key Actions Taken: 
- Hardened password policies across Linux and Windows systems
- Reset and rotated all user credentials
- Adjusted pfSense firewall rules to restrict unnecessary inbound traffic
- Monitored logs and alerts using Wazuh and Security Onion

🚨 Attacks Detected: 
- Nmap network reconnaissance
- Brute-force login attempts (50+ failures in 24 hours)
- Invalid HTTP headers and chunked encoding (Snort alerts)

🧰 Tools Used: 
- Security Onion: Network intrusion detection & alert monitoring
- Wazuh: File integrity monitoring, login attempt detection, vulnerability scanning
- pfSense: Firewall rule enforcement and suspicious traffic logging

🔒 Recommendations: 
- Enforce MFA for all users
- Implement centralized password management
- Conduct quarterly phishing and security awareness training
- Audit password compliance and access policies regularly
