# Acceptable Use Policy (AUP)

**Version:** 1.0  
**Owner:** Home Lab Administrator-Faith Ndu  
**Applicability:** All users and automated processes within the Home Lab domain.

## 1. Purpose
This policy outlines the acceptable use of computing resources within the SOC/GRC Home Lab. These rules are enforced to protect the integrity of the host workstation (ASSET-01) and maintain compliance with privacy baselines over the shared apartment wireless infrastructure.

## 2. Authorized Use
* **Educational Purpose:** Resources must be used strictly for cybersecurity research, industry self-study, and portfolio development.
* **Isolation:** All automated attack scripts or active scanning tools must run within network-isolated environments behind the travel router.
* **Approved Toolsets:** Execution of Splunk, Sysmon, and Atomic Red Team payloads is restricted to designated target subnets.

## 3. Prohibited Use
* **Upstream Disruption:** Automated scripts or testing tools must not consume 100% of host CPU/RAM resources to preserve system stability.
* **Neighbor Privacy Violations:** Targeting, scanning, or attempting to intercept traffic from other residents sharing the apartment Wi-Fi is strictly prohibited and violates local privacy laws.
* **External Attacks:** Utilizing lab infrastructure to launch unauthorized traffic against external internet entities is strictly forbidden.

## 4. Security Requirements
* **Credential Hygiene:** Lab virtual machines must use dedicated passwords distinct from real-world personal assets.
* **Transport Encryption:** Administrative pathways (RDP/SSH) initiated across untrusted segments must use encrypted VPN tunnels via Tailscale.
* **Patch Cycle:** Security updates must be applied to the primary monitoring instances at least once per calendar month.
