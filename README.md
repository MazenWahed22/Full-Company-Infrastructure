# 🎓 Networking Simulation Lab – Full Company Infrastructure

## 📘 Project Overview

This project simulates a **full company infrastructure** with **two branches (Cairo & Alexandria)** connected through an ISP using **Frame Relay**. The design ensures scalability, segmentation, and real-world best practices in enterprise networking.

---

## 🌐 Connectivity

* **Frame Relay** used to connect Cairo & Alexandria branches.
* Each branch connected via a **router** linked to a **Layer 3 switch**, then to **two Layer 2 switches**.
* Each Layer 2 switch connects to **two end devices** (total of 9 devices across the whole network).

---

## 🧠 Addressing & VLANs

* **DHCP Server** deployed in the **Cairo branch**.
* **ip helper-address** configured on the Alexandria router to forward DHCP requests.
* **5 VLANs** created → each device assigned to a different VLAN.
* **Inter-VLAN Routing** configured on the **Layer 3 Switch**.
* **Default gateways** assigned per VLAN for proper communication.

---

## 🛡️ Security Implementation

* **Access Control Lists (ACLs)** applied for traffic filtering.
* **ICMP blocking** from specific hosts to the server ( Vlan 2 + PC 6 + PC 7 ) .
* Only **authorized VLANs** allowed access to specific services.

---

## ⚙️ Other Features

* **EtherChannel** configured between the **Layer 3 switch** and each **Layer 2 switch** (2 physical links per connection).
* **EIGRP** enabled for **dynamic routing** across both branches.
* **Trunk Links** configured between switches for proper VLAN propagation.
* Network design follows **real-world standards** and ensures **future scalability**.

---

## 📐 Network Topology (Summary)

* **Branch 1 (Cairo)** → Router0, Layer 3 Switch + 2 Layer 2 Switches, DHCP server, 5 VLANs, multiple PCs.
* **Branch 2 (Alexandria)** → Router1, Switch + PCs + Server.
* **ISP (Frame Relay)** → Provides WAN connectivity.
* **Dynamic Routing (EIGRP)** → Ensures automatic route exchange.

---
  
## 📜 Author
**Mazen Wahed**  
- 💼 [LinkedIn Profile](https://www.linkedin.com/in/mazen-wahed-260826320)  
- 📧 mazenwahed538@gmail.com  




