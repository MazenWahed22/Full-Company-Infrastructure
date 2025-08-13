# Full-Company-Infrastructure
# 🏢 Networking Simulation Lab – Full Company Infrastructure

## 📌 Project Overview
This project is a **complete company network simulation** built using **Cisco Packet Tracer**.  
It simulates a company with **two branches** (Cairo & Alexandria) connected using **Frame Relay**, featuring VLAN segmentation, inter-VLAN routing, DHCP, ACLs, EtherChannel, and dynamic routing with EIGRP.

---

## 🌐 Network Topology
**Branches:**
- **Cairo Branch**:
  - Router connected to a Layer 3 Switch
  - Layer 3 Switch connected to two Layer 2 Switches
  - DHCP Server deployed locally

- **Alexandria Branch**:
  - Router connected to a Layer 3 Switch
  - Layer 3 Switch connected to two Layer 2 Switches
  - Uses DHCP relay via `ip helper-address`

---

## 🧠 Addressing & VLANs
- **4 VLANs**: Each device assigned to a separate VLAN
- **DHCP Server**: Located in Cairo, serving both branches
- **Inter-VLAN Routing**: Configured on the Layer 3 Switch
- **Default Gateways**: Assigned for all VLANs

---

## 🛡️ Security Configuration
- **ACLs** to enforce network policies:
  - Block ICMP from specific hosts to the server
  - Prevent VLAN 2 from accessing the server via HTTP (port 80)
  - Restrict access to certain services for unauthorized VLANs

---

## ⚙️ Additional Features
- **EtherChannel**: Implemented between Layer 3 switch and Layer 2 switches (two physical links per connection)
- **EIGRP**: Configured for dynamic routing between branches
- **Trunk Links**: Enabled between switches for VLAN propagation

---

## 📂 Project Files
- `.pkt` file: Cisco Packet Tracer project file containing full configuration
- `README.md`: Project documentation (this file)

---

## 📸 Screenshots
*(Add topology and configuration screenshots here)*

---

## 🚀 How to Use
1. Open the `.pkt` file in **Cisco Packet Tracer** (v8.x or later).
2. Explore the network topology and configurations.
3. Test VLAN segmentation, routing, ACLs, and connectivity.

---

## 📜 Author
**Mazen Wahed**  
- 💼 [LinkedIn Profile](https://www.linkedin.com/in/mazen-wahed-260826320)  
- 📧 mazenwahed538@gmail.com  

