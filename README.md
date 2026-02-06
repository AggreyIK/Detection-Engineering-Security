# Detection Engineering & Security Monitoring.

This repository documents the end-to-end design, deployment, and operation of a realistic enterprise Security Operations Center (SOC) lab. The project simulates a corporate environment with centralized identity management, multiple Windows endpoints across headquarters and branch locations, attacker activity, and a fully functional SIEM/EDR platform for detection and response.

The lab is built to reflect real-world SOC workflows, progressing from infrastructure and identity engineering to endpoint visibility, attack detection, dashboarding, and incident investigation. All phases are implemented hands-on and supported with technical documentation and evidence.

---

# Focus

- Map detections to MITRE ATT&CK techniques
- Build behavioral detections (not just signatures)
- Detection lifecycle: build → test → tune → measure
- Purple team feedback loop

---

## Project Scope & Objectives

- Design and deploy an enterprise-style virtual network
- Implement Active Directory for centralized identity and authentication
- Deploy multiple Windows endpoints across HQ and branch locations
- Centralize security logging and endpoint telemetry
- Implement SIEM and EDR capabilities using Wazuh
- Simulate real-world attack techniques in a controlled environment
- Develop and tune custom detection rules mapped to MITRE ATT&CK
- Build SOC dashboards for monitoring and triage
- Document incident investigations and response actions

---

## Lab Architecture

**Environment Components**
- Windows Server Domain Controller (Active Directory & DNS)
- Windows 10 endpoints (HQ and Branch offices)
- Wazuh Server (SIEM, EDR, and security analytics)
- Sysmon for enhanced endpoint telemetry
- Kali Linux attacker machine for threat simulation

The environment uses isolated internal networking with static IP addressing and enterprise-style segmentation to mirror a production SOC deployment.

---

## Technologies Used

- Windows Server (Active Directory, DNS)
- Windows 10 Enterprise Endpoints
- Wazuh (SIEM & EDR)
- Sysmon
- Parrot VM
- VMware (virtualization - Type 2 Hypervisor)

---

## Project Phases

### Phase 1 – Infrastructure & Virtualization
- Designed the SOC lab topology
- Deployed all virtual machines
- Implemented isolated enterprise networking
- Prepared scalable infrastructure for SOC operations

---

### Phase 2 – Active Directory & Identity Management
- Deployed Windows Server Domain Controller
- Created corporate domain (`infoknox.local`)
- Configured DNS and directory services
- Created enterprise user accounts and roles
- Joined all endpoints to the domain

---

### Phase 3 – Endpoint Integration
- Integrated HQ and Branch workstations into the domain
- Verified centralized authentication
- Established enterprise endpoint baselines

---

### Phase 4 – Endpoint Visibility & Logging
- Installed Sysmon for advanced endpoint telemetry
- Deployed Wazuh agents to all endpoints
- Centralized Windows security and system logs
- Verified real-time log ingestion into SIEM

---

### Phase 5 – Attack Simulation & Detection
- Simulated attacker techniques including:
- Password brute force
- PowerShell abuse
- Active Directory reconnaissance
- Persistence via scheduled tasks
- Mass file creation (ransomware-like behavior)
- Observed and validated detections in Wazuh

---

### Phase 6 – Detection Engineering & Tuning
- Created custom Wazuh detection rules
- Implemented frequency-based and behavior-based detections
- Mapped detections to MITRE ATT&CK techniques
- Tuned alerts to reduce false positives

---

### Phase 7 – SOC Dashboards
- Built SOC dashboards for:
- Active alerts over time
- High-severity alert queue
- Top attacked hosts
- Targeted user accounts
- MITRE ATT&CK technique coverage
- HQ vs Branch activity comparison

---

### Phase 8 – Incident Investigation & Reporting
- Documented security incidents detected in the lab
- Performed basic investigation and analysis
- Recorded findings, impact, and remediation steps
- Produced SOC-style incident reports

---

## Key Skills Demonstrated

- Enterprise infrastructure design
- Active Directory administration
- Endpoint logging and telemetry engineering
- SIEM & EDR deployment
- Detection engineering and alert tuning
- MITRE ATT&CK alignment
- SOC dashboard creation
- Incident investigation and documentation

---

## Disclaimer

!!All attack simulations were performed in a controlled lab environment for educational and defensive security purposes only!!
