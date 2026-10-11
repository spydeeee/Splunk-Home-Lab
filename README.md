# Splunk-Home-Lab

## Objective
[Brief Objective - Remove this afterwards]

🔧 Project: Local SOC Lab — Splunk SIEM Setup

Built a fully functional local SOC (Security Operations 
Center) lab from scratch following industry best 
practices, using:

🖥️ Stack:
• Splunk — Central SIEM & SOC Dashboard
• Ubuntu Linux — Server/monitoring node
• Windows 10 — Monitored endpoint (alert source)
• Kali Linux — Attack simulation node
• Oracle VirtualBox — Virtualization platform

✅ What I did:
• Set up Splunk as the SIEM to receive and index 
  security events from a Windows 10 machine
• Configured log forwarding from Windows 10 to the 
  Splunk dashboard
• Monitored and analyzed real-time security alerts 
  on the SOC dashboard
• Simulated attacks using Kali Linux to generate 
  detectable events in Splunk
• Practiced log search, filtering, and alert 
  investigation using Splunk's interface

💡 Why this matters:
This project complements my existing Wazuh SIEM home 
lab — giving me hands-on experience across TWO 
industry-standard SIEM platforms (Wazuh + Splunk), 
which is directly relevant to SOC L1 Analyst roles.


### Skills Learned
[Bullet Points - Remove this afterwards]

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
[Bullet Points - Remove this afterwards]

- Security Information and Event Management (Splunk) Splunk system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools (log forwarding from Windows 10)to create realistic network traffic and attack scenarios.

## Steps

*Ref 1: <img width="1068" height="849" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/5e41ca13-c844-4e05-a703-be205a1f60d0" />
         Step 1 — Start Splunk Enterprise
Screenshot: 01-splunk-startup.png
Start the Splunk service on your Linux machine and wait for the web interface to become available. Your terminal screenshot shows the startup process completing successfully.
Expected result: Splunk Web is accessible on port 8000.
*Ref 2: <img width="964" height="646" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/509bce04-ce9e-456a-8533-603da19842fc" />


