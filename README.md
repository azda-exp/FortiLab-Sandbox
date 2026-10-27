# FortiLab-Sandbox
# 🛡️ FortiLab Sandbox - Enterprise Firewall & Network Topology

Welcome to my network security and firewall operations lab repository. This lab is built and tested using **EVE-NG**, **FortiGate VM**, and virtual network endpoints to practice real-world enterprise firewall configuration, routing, and defensive architecture.

---

## 🏗️ Topology Architecture

- **Firewall:** FortiGate-VM64-KVM
- **Switch:** Cisco IOL Layer 2 Switch (`SW1`)
- **Endpoint:** Virtual PC Simulator (`VPC`)
- **Platform:** EVE-NG on Ubuntu / VirtualBox

---

## 🔌 IP Addressing & Interface Mapping

| Device | Interface | IP Address / Subnet | Role / Description |
| :--- | :--- | :--- | :--- |
| **FortiGate** | `port1` | `192.168.2.1/24` | LAN Gateway (Connected to SW1 / VPC) |
| **FortiGate** | `port2` | `DHCP` | WAN / Upstream Management Interface |
| **VPC** | `eth0` | `192.168.2.10/24` | Internal Test Host |

---

## 🚀 Lab Objectives & Configuration Highlights

1. **Initial Hardening & Access Control:**
   - Admin password reset and secure CLI access configured.
   - Interface management access enabled (`ping`, `ssh`, `http`, `https`).
2. **L2/L3 Connectivity Verification:**
   - Established internal routing between virtual endpoint (`192.168.2.10`) and firewall gateway (`192.168.2.1`).
3. **Configuration Export:**
   - Full device configuration stored in `fortigate-config.cfg`.

---

## 🛠️ How to Use

1. Clone the repository:
```bash
   git clone https://github.com/YOUR-USERNAME/FortiLab-Sandbox.git
   
    Import the .unl topology file into your EVE-NG environment.
    Load the configuration file into your FortiGate instance.

Maintained by Prince (Hacker / Network Engineer)
PRINCE
