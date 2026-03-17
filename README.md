# 🌐 IP Addressing and Subnetting Implementation

## 📌 Project Description
This project demonstrates how to design and implement an IP addressing scheme using subnetting. The network is divided into multiple subnets to improve efficiency and communication between different departments.

---

## 🎯 Objective
- To understand IP addressing and subnetting
- To divide a network into smaller subnets
- To configure a router and PCs in Cisco Packet Tracer
- To test connectivity using ping command

---

## 🛠️ Tools Used
- Cisco Packet Tracer

---

## 🏢 Network Design
The network consists of 3 departments:
- switch1
- switch2
- switch3

Each department is connected using:
- 1 Router
- 3 Switches
- Multiple PCs

---

## 🌍 IP Addressing Scheme

### Base Network:
192.168.1.0/24

### Subnet Mask:
/26 (255.255.255.192)

---

### 🟢 switch1 Network
- Network: 192.168.1.0/26
- Gateway: 192.168.1.1
- PCs:
  - 192.168.1.2
  - 192.168.1.3

---

### 🔵 switch2 Network
- Network: 192.168.1.64/26
- Gateway: 192.168.1.65
- PCs:
  - 192.168.1.66
  - 192.168.1.67

---

### 🟡 switch3 Network
- Network: 192.168.1.128/26
- Gateway: 192.168.1.129
- PCs:
  - 192.168.1.130
  - 192.168.1.131

---

## ⚙️ Router Configuration
enable
configure terminal

interface gig0/0
ip address 192.168.1.1 255.255.255.192
no shutdown

interface gig0/1
ip address 192.168.1.65 255.255.255.192
no shutdown

interface gig0/2
ip address 192.168.1.129 255.255.255.192
no shutdown

## 🧪 Testing
Connectivity is verified using the ping command between different PCs.

Example: 192.168.1.130
          192.168.1.3



---

## 📸 Screenshots Included
- Network Topology
- Subnetting Calculation
- Router Configuration
- PC Configuration
- Ping Test Results

---

## 📂 Project Structure
IP-Subnetting-Project/
│
├── IP_Subnetting_ViralSolkar.pkt
├── README.md
├── subnetting-calculation.txt
├── screenshots/


---

## ✅ Conclusion
The network was successfully divided into subnets using a /26 subnet mask. All devices were configured correctly, and communication between different subnets was verified successfully.

---

## 👨‍💻 Author
Viral Solkar


