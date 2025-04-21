# Simulating EDR with LimaCharlie Victim-Attacker VMs and Sliver-C2 Framework

I have worked on a home lab using blog posts and simulated Endpoint Detection and
Response(EDR) system which consists of a Windows 10 victim virtual(VM) machine,
Linux attacker VM, and LimaCharlie with EDR-like ability. Installed a sensor on the victim
machine that collects and analyzes log files and, after simulating attacks using Sliver C2 a
command and control framework, created detection rules leveraging the Sigma rule to
identify and block abnormal activities. Fine-tuned the detection rules to minimize false
positives, enhancing the system’s threat detection and prevention capabilities.


## Lab Components

- Victim VM: Windows 10 with LimaCharlie Sensor
- Attacker VM: Linux (Kali/Ubuntu) running Sliver C2 Framework
- EDR Platform: [LimaCharlie](https://limacharlie.io/)
- Detection Logic: Custom Sigma rules

## Attack Simulation

Used [Sliver C2](https://github.com/BishopFox/sliver) to simulate attacks like:
- Reverse shell
- File exfiltration
- Persistence mechanisms
- Privilege escalation

## Detection & Response

- Created Sigma rules to detect suspicious behavior
- Fine-tuned rules to reduce false positives
- Leveraged LimaCharlie’s rule engine to trigger detections based on logs

## Project Layout

- `victim-vm/` – Sensor install steps, attack logs
- `attacker-vm/` – Sliver setup and attack commands
- `detection-rules/` – Custom Sigma rules
- `logs/` – Captured logs from simulated attacks




