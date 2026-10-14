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


###Phase 1 — SIEM setup and log ingestion
[Document existing work]
- Splunk Enterprise setup
- Windows Forwarder service
- Windows Security and Application logs
- Basic SPL searches


## Steps

*Ref 1: Start Splunk Enterprise
Screenshot: 
Start the Splunk service on your Linux machine and wait for the web interface to become available. Your terminal screenshot shows the startup process completing successfully.
Expected result: Splunk Web is accessible on port 8000.
<img width="1068" height="849" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/5e41ca13-c844-4e05-a703-be205a1f60d0" />
        
*Ref 2: Verify the Windows Forwarder
Screenshot:
Use PowerShell to check the Splunk Universal Forwarder service. Your screenshot shows an initial service error followed by a successful Running status.
Expected result: The service runs and is configured to forward the intended Windows logs.
<img width="1011" height="604" alt="WhatsApp Image 2026-10-11 at 7 23 49 PM" src="https://github.com/user-attachments/assets/33d7304d-8542-485c-bc2f-2dc4ed892350" />


*Ref 3: Validate the Lab Host
Screenshot: 
Use Kali Linux to perform a basic network check against a system you own or have permission to test. The supplied screenshot shows a reachable host and filtered TCP ports.
Expected result: Record the scan findings. Filtered ports do not prove that a service is open.
<img width="831" height="651" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/d08f41e1-a1fe-4f8e-ac0b-1dbc5c83089d" />



*Ref 4: Search Windows Security Events
Screenshot:
In Splunk Search, run the query below to locate events in your Windows index.
index="windows" sourcetype="WinEventLog:Security"
<img width="1012" height="869" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/8e61c26c-d208-4a95-a563-8c40bc94157d" />

*Ref 5: Review Application Events
Screenshot: 
Review your Application log results and inspect fields such as EventCode, LogName, and ComputerName.
index="windows" sourcetype="WinEventLog:Application"
<img width="1160" height="856" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/fa404aac-f660-4d97-adb8-dffdec1391cf" />


## References
- **Video Guide**: [What is Splunk) | Get Splunk FREE Today! (Defronix Academy)]([http://www.youtube.com/watch?v=MI5DMKuxhH0](https://www.youtube.com/live/Gd5a47UaRY4?si=5Ew3PWTdqP6gdcIz)) 
- **Portfolio Template**: [MyDFIR Detection-Lab Template](https://github.com/Test-MyDFIR/Detection-Lab/blob/main/README.md)



