# Overview
This project documents the design, deployment, and compromise of a simulated enterprise Active Directory environment.

The lab was built to practice real-world red team and penetration testing techniques against Windows domain infrastructure, focusing on credential abuse, lateral movement, and privilege escalation.

All attacks were executed in an isolated host-only virtual lab.

## Lab Architecture

<div align="center">
  <img src="images/diagram.png" alt="Active Directory Lab Diagram" width="600" />  
</div>

<div style="text-align: justify; max-width: 600px; margin: auto; align="center";>
  
  *Network topology for the Active Directory lab environment. NORTHSHORE.local is the lab domain. The Domain Controller (WATCHTOWER-DC) manages the lab, and the two workstations (PIER01 and PIER02) simulate typical user machines. IP addresses are private lab subnets. This diagram helps visualize attack paths and protocol interactions.* 

</div>

### Environment

- 1 Domain Controller (Windows Server)
- 2 Domain-Joined Windows Clients
- 1 Attacker Machine (Kali Linux)

### Domain Setup

- Custom AD domain (NORTHSHORE.local)
- Multiple user accounts (standard + service accounts)
- Misconfigurations intentionally introduced for exploitation practice


## Attack Scenarios

### Initial Attack Vectors

- [LLMNR Poisoning](01-llmnr-poisoning/README.md)

### Enumeration

### Post-Exploitation


**Ethical Disclaimer**
This lab was created and attacked in a privately owned, isolated environment for educational and professional development purposes only.
