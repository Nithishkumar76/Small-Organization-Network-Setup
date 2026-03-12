# 🏢 Small Organization Network Setup using VLAN and Router-on-a-Stick

## 📌 Project Overview
This project simulates a small organization network infrastructure using Cisco Packet Tracer.

The network is divided into different departments using VLAN segmentation, and communication between VLANs is enabled using Router-on-a-Stick Inter-VLAN routing.

The design demonstrates how organizations logically separate departments while maintaining network connectivity.

--------------------------------------------------

## 🧰 Network Technologies Used
- 🧩 VLAN (Virtual LAN)
- 🔀 Router-on-a-Stick
- 🔗 Trunk Configuration
- 🖥 Access Ports
- 📡 Wireless Access Points
- 🌐 IP Addressing and Subnetting
- 🔁 Inter-VLAN Routing

--------------------------------------------------

## 🌐 Network Topology

The network consists of three departments.

### 🏢 VLAN 10 – Admin Department
Network Address: 192.168.1.0/26

Devices
- 🖥 PC
- 🖨 Printer
- 📡 Wireless Access Point
- 💻 Laptop
- 📱 Smartphone

--------------------------------------------------

### 💰 VLAN 20 – Finance Department
Network Address: 192.168.1.64/26

Devices
- 🖥 PC
- 🖨 Printer
- 📡 Wireless Access Point
- 💻 Laptop
- 📱 Smartphone

--------------------------------------------------

### 🛎 VLAN 30 – Reception Department
Network Address: 192.168.1.128/26

Devices
- 🖥 PC
- 🖨 Printer
- 📡 Wireless Access Point
- 💻 Laptop
- 📱 Smartphone

--------------------------------------------------

## 🖧 Core Devices Used
- 📡 1 Router – Used for Inter-VLAN routing
- 🔀 1 Switch – Used for VLAN configuration
- 📶 3 Wireless Access Points
- 💻 End devices (PCs, printers, laptops, smartphones)

--------------------------------------------------

## 🏗 Network Design

### 🧩 VLAN Segmentation
Each department is separated using VLANs to reduce broadcast traffic and logically organize the network.

VLAN    Department    Network
10      Admin         192.168.1.0/26
20      Finance       192.168.1.64/26
30      Reception     192.168.1.128/26

--------------------------------------------------

### 🔀 Router-on-a-Stick
Inter-VLAN communication is achieved using router subinterfaces.

Router Interface: G0/0

G0/0.10 → VLAN 10  
G0/0.20 → VLAN 20  
G0/0.30 → VLAN 30  

Each subinterface acts as the default gateway for its VLAN.

--------------------------------------------------

### 🔗 Trunk Configuration
The link between the switch and router is configured as a trunk to carry multiple VLANs.

Switch Port → Trunk Mode  
Allowed VLANs → 10,20,30

--------------------------------------------------

## 🧪 Network Testing

Connectivity tests were performed between devices in different VLANs.

✅ Admin → Finance communication: Successful  
✅ Admin → Reception communication: Successful  
✅ Finance → Reception communication: Successful  

This confirms that Inter-VLAN routing is working correctly.

--------------------------------------------------

## 🎯 Skills Demonstrated
- 🧩 VLAN configuration
- 🔌 Switch port assignment
- 🔗 Trunk configuration
- 🔀 Router-on-a-Stick setup
- 🏗 Network topology design
- 🛠 Connectivity troubleshooting

--------------------------------------------------

## 🛠 Tools Used
💻 Cisco Packet Tracer

--------------------------------------------------

## 👨‍💻 Author
Nithish Kumar