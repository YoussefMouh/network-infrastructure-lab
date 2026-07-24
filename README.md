# 🏢 Enterprise Network Infrastructure — PFE 2025/2026

> **Licence Professionnelle ACSRI** — ENSET Mohammedia, Université Hassan II  
> **Réalisé par :** Youssef MOUHIM | **Encadrant :** Pr. Azeddine KHIAT

---

## 📌 Overview

Simulation of a complete enterprise IT infrastructure for **Upline Group** (upline.ma),
built on PNetLab with real-world components:
FortiGate firewall, Cisco routing/switching, Windows Server AD, GLPI ITSM, and Zabbix monitoring.

---

## 🗺️ Network Architecture

![Topology](screenshots/topology_pnetlab.png)

| Zone | Subnet | Components |
|------|--------|------------|
| WAN  | DHCP   | FortiGate port1 |
| LAN  | 192.168.2.0/24 | AD, GLPI, Zabbix, Clients |
| DMZ  | 192.168.3.0/24 | (reserved) |

---

## 🛠️ Tech Stack

| Component | Technology | Version |
|-----------|-----------|---------|
| Firewall | FortiGate | FortiOS 7.x |
| Routing | Cisco IOS | R1, R2 (Router-on-a-Stick) |
| Switching | Cisco IOS | SW1, SW2 (VLAN10) |
| Identity | Windows Server AD | 2019, domain upline.ma |
| ITSM | GLPI | 10.0.15 (HTTPS) |
| Monitoring | Zabbix | 6.4 (SNMP) |
| Emulator | PNetLab | — |

---

## ✅ Features Implemented

- [x] FortiGate WAN/LAN/DMZ segmentation with firewall policies
- [x] VLAN10 with Router-on-a-Stick (R1/R2)
- [x] Active Directory domain (upline.ma) with users/OUs
- [x] GLPI 10 with LDAP/AD authentication (RBAC)
- [x] GLPI HTTPS (self-signed cert, MTU 1400 fix)
- [x] GLPI Agent inventory on Windows 10 clients
- [x] Realistic helpdesk ticket data (SQL injection)
- [x] Zabbix 6.4 monitoring all 8 devices via SNMP
- [x] Full SNMP configuration on FortiGate + Cisco devices

---

## 📸 Screenshots

| GLPI Dashboard | Zabbix Monitoring |
|---|---|
| ![GLPI](screenshots/glpi_inventory.png) | ![Zabbix](screenshots/zabbix_monitoring.png) |

---

## 📄 Documentation

- 📘 [Rapport PFE (PDF)](docs/rapport_PFE_MOUHIM.pdf)
- 📊 [Slides Soutenance](docs/soutenance_slides.pptx)

---

## 👤 Author

**Youssef MOUHIM** — IT Administrator @ Upline Group | ENSET Mohammedia 2026  
[![GitHub](https://img.shields.io/badge/GitHub-MrSymbatox-black?logo=github)](https://github.com/MrSymbatox)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://linkedin.com/in/youssef-mouhim)
