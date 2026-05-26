# Hybrid SOC & GRC Home Lab Cyber Security Portfolio

## Overview
This repository documents the architecture, implementation, and auditing of a hybrid home lab environment designed for SOC Analysis and IT GRC (Governance, Risk, and Compliance). The lab focuses on the Australian Signals Directorate (ASD) Essential Eight framework and real-time threat detection using industry-standard tools.

## Infrastructure Architecture
* **Physical Environment:** Shared Apartment Network (Wi-Fi 6)
* **Network Isolation Control:** To mitigate risks associated with a shared infrastructure environment, a high-throughput GL-MT3000 (Beryl AX) Wi-Fi 6 router is deployed in Repeater Mode to establish an isolated, firewalled private LAN (`192.168.8.0/24`).

### Asset Register


| Asset ID | Device | Role | Specs |
| :--- | :--- | :--- | :--- |
| **ASSET-01** | Dell Inspiron 14 | Management / GRC Workstation | i7 13th Gen, 16GB RAM (Fixed/Soldered) |
| **ASSET-02** | Dell OptiPlex 7090 Micro | SOC Server (Headless) | i5-11500T (6 Cores), 16GB RAM, 256GB SSD |
| **NET-01** | GL-MT3000 (Beryl AX) | Perimeter Firewall Router | Wi-Fi 6 Pocket Gateway / OpenWrt |
| **NET-02** | Tailscale | Secure Remote Access | Software-Defined VPN / Overlay Network |

## Lab Components

### SOC Operations (Technical)
* **SIEM:** Splunk Enterprise / Wazuh for centralized log management and analytics.
* **Telemetry:** Microsoft Sysmon and Windows Event Forwarding.
* **Attack Simulation:** Invoke-AtomicRedTeam for generating forensic artifacts.

### IT GRC (Process & Governance)
* **Audit Framework:** ASD Essential Eight Maturity Model.
* **Vulnerability Management:** Vulnerability assessment scans of internal assets.
* **Documentation Suite:** Governance policies and active risk monitoring.

## Portfolio Documentation Links
* [View Active Risk Register](./projects/risk-register.md)
* [View Acceptable Use Policy (AUP)](./projects/acceptable-use-policy.md)

## Skills Demonstrated
* **Tools:** Splunk, Sysmon, PowerShell, VMware / Proxmox, Tailscale.
* **Frameworks:** ASD Essential Eight, NIST CSF, ISO 27001.
* **Technical Writing:** Policy drafting, Audit reporting, and Risk Assessment.
