# University Network Infrastructure & Services

This repository hosts a complete simulation of a **University Campus Network** designed in **Cisco Packet Tracer**. The project focuses not just on connectivity, but on deploying essential network services (Servers) required for an academic environment.

**Project Scope:** University Network Design & Server Configuration
**Tool Used:** Cisco Packet Tracer

##  Network Topology
The architecture mimics a real-world campus with distinct zones (e.g., Admin Building, Student Dorms, Library) connected via a robust Core/Distribution/Access layer model.

##  Key Configurations

### 1. Server Administration (Key Feature)
This simulation includes fully configured servers to demonstrate Layer 7 services:
* ** Email Server:** Configured SMTP/POP3 services allowing users (Faculty/Students) to send and receive emails within the domain (e.g., `user@university.edu`).
* ** Web Server (HTTP):** Hosted university website accessible by all end clients via domain name.
* ** DNS Server:** Implemented to resolve domain names (URL) to IP addresses for the Web and Email servers.
* ** DHCP Server:** Automatic IP allocation for student and staff devices to ensure plug-and-play connectivity.

### 2. Switching & LAN Design
* **VLAN Segmentation:** Traffic isolation for different departments (Faculty VLAN, Student VLAN, Management VLAN).
* **Security:** Port Security enabled on access switches to prevent unauthorized device access.
* **VTP & Trunking:** Efficient VLAN management across multiple switches.

### 3. Routing & Connectivity
* **Inter-VLAN Routing:** Configured (Router-on-a-Stick or L3 Switch) to allow communication between students, faculty, and servers.
* **Routing Protocol:** (Choose one: OSPF / EIGRP / RIP) configured for dynamic path selection and redundancy.

##  How to Test the Services
1.  **Email:** Open a PC in the topology, go to the **Desktop > Email** tool, and try sending an email from `Student1` to `Professor1`.
2.  **Web Access:** Open the **Web Browser** on any PC and type the university URL (e.g., `www.university.edu`).
3.  **Connectivity:** Use the Command Prompt to `ping` the Server Farm from different VLANs.

---
*Project designed by Parniyan Malekzadeh.*
