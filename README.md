# Enterprise-Network-Simulation
A comprehensive networking lab designed to simulate an enterprise-grade infrastructure across multiple campuses, focusing on scalability, redundancy, secure connectivity, and service availability. This project aimed to strengthen practical skills in network architecture, security implementation, and device configuration using Cisco technologies.
____________________________________________________________________________________________________________________________________________________
# 🏛️ Enterprise Network Simulation Project

An extensive, real-world enterprise network simulation lab developed to reinforce practical skills in network architecture, infrastructure security, and service deployment. The lab reflects a multi-campus layout and addresses business needs for scalability, redundancy, and secure communication.

## 📘 Lab Source
Developed under **GURUTECH NETWORKS**

## 🧭 Objectives

- Design and implement a hierarchical network topology: Core, Distribution, and Access layers  
- Deploy services in a fortified DMZ, including DHCP, DNS, FTP, WEB, Email, and SMTP  
- Ensure secure connectivity for branch users to access centralized resources  
- Achieve redundancy via dual ISPs (SEACOM & Safaricom), DHCP failover, EtherChannel, and HSRP  
- Secure network traffic using ACLs, static routing, and Cisco ASA Firewall configurations  
- Enable centralized wireless control, VoIP telephony, and remote administrative access via SSH  

## 🛠️ Technologies & Tools

- **Platform:** Cisco Packet Tracer  
- **Routing Protocol:** Open Shortest Path First (OSPF)  
- **Switches:** Catalyst 3850 (48-port), Catalyst 2960 (48-port)  
- **Firewall:** Cisco ASA 5500-X Series  
- **Wireless:** Wireless LAN Controllers (WLC), Lightweight Access Points (LAPs)  
- **VoIP:** Cisco Voice Gateway, IP Phones  
- **Virtualization:** Two physical servers hosting multiple VMs for service deployment  
- **Security Features:** STP PortFast, BPDUguard, SSH ACLs, static addressing in server farm  
- **Link Aggregation:** EtherChannel via LACP  

## 🌐 IP Address Planning

| **Function**       | **IP Range**           |
|--------------------|------------------------|
| Management Network | `192.168.10.0/24`      |
| WLAN               | `10.20.0.0/16`         |
| LAN                | `172.16.0.0/16`        |
| VoIP               | `172.30.0.0/16`        |
| DMZ                | `10.11.11.0/27`        |
| Public ISP 1       | `105.100.50.0/30`      |
| Public ISP 2       | `197.200.100.0/30`     |

## 🧩 Core Features

- Hierarchical topology with logical separation of traffic  
- VLAN IDs: `10` (Management), `20` (LAN), `50` (WLAN), `70` (VoIP), `199` (Blackhole for unused ports)  
- DHCP failover and dynamic IP provisioning  
- DNS, FTP, Email, and Web services in virtualized DMZ environment  
- VoIP communication across departments using IP phones and voice gateway  
- Wireless coverage via departmental LAPs managed by a central WLC  
- Cloud computing readiness for remote client access  

## 🔐 Security Measures

- Cisco ASA Firewall configured with security zones, static routes, and inspection policies  
- Access Control Lists (ACLs) restricting SSH access to senior admin systems  
- Password encryption, console and enable passwords, banner messages, and IP domain lookup disabled  
- BPDUguard and STP PortFast enabled for rapid switch port transitions and protection  
- Subnetting for precise IP allocation across departments  
- HSRP for load balancing and high availability of gateways

## ✅ Final Validation

Comprehensive testing confirmed device communication, service reachability, protocol convergence, and redundancy effectiveness — ensuring the simulated network meets business requirements and is future-proofed for scale and security.



