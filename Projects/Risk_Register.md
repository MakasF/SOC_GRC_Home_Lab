# Home Lab Risk Register

**Scope:** Hybrid SOC/GRC Home Lab Environment  
**Framework Context:** Risk Assessment for Procurement and Architecture  

## 1. Risk Matrix Reference


| Likelihood / Impact | Low (1) | Medium (2) | High (3) |
| :--- | :--- | :--- | :--- |
| **High (3)** | 3 (Medium) | 6 (High) | 9 (Critical) |
| **Medium (2)** | 2 (Low) | 4 (Medium) | 6 (High) |
| **Low (1)** | 1 (Low) | 2 (Low) | 3 (Medium) |

## 2. Active Risk Log


| ID | Risk Description | Category | Likelihood | Impact | Score | Mitigation Strategy | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **R-01** | **Resource Constraints:** Original laptop hardware profile (soldered RAM) restricts high-compute SIEM operations. | Technical | 1 | 1 | **1** | **Mitigate:** Procured ASSET-02 (Dell 7090 6-Core) to offload heavy workloads. | Closed |
| **R-02** | **Unauthorized Access (Shared Wi-Fi):** Shared apartment network allows potential lateral movement or data sniffing from other tenants. | Security | 1 | 3 | **3** | **Avoid:** Implemented GL-MT3000 (Beryl AX) Wi-Fi 6 Router and Tailscale to build a micro-segmented network. Hardware upgraded for improved WireGuard VPN throughput. | Managed |
| **R-03** | **Data Loss (Single Disk):** Failure of the single SSD on assets leads to loss of lab configurations and code. | Operational | 1 | 3 | **3** | **Reduce:** Automate backups of environment configuration files directly to this GitHub repository. | Open |
| **R-04** | **Power Instability:** Voltage surge or blackouts in apartment cause "dirty shutdown" and database corruption. | Physical | 2 | 2 | **4** | **Accept:** Cost of an enterprise UPS exceeds lab financial value; accept risk and rely on fresh rebuild scripts. | Accepted |
| **R-05** | **Lack of Physical Display:** Loss of direct console viewing capability during host OS or hypervisor failures. | Operational | 2 | 2 | **4** | **Reduce:** Configured out-of-band management via Tailscale. Planned physical hardware reserve for portable monitor. | Managed |
