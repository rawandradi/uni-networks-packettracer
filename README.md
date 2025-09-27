# Computer Networks Project #2 – Cisco Packet Tracer

## 📌 Overview
This project was developed as part of the **Computer Networks (ENCS3320)** course at **Birzeit University**.  
It focuses on the design and implementation of a **complete IP-based network** using **Cisco Packet Tracer**.  

The network is divided into five main areas:
- **Core (Area 0)** – Backbone, interconnects all areas using OSPF.  
- **University (Area 1)** – PCs, servers, DHCP, and wireless access.  
- **Street (Area 2)** – Cell tower, smartphones, and central office server.  
- **Home (Area 3)** – PCs with static IPs simulating a home environment.  
- **Datacenter (Area 4)** – Web, Mail, and DNS servers.  

Key services and protocols include:
- **DHCP** (dynamic IP allocation)  
- **DNS** (domain resolution)  
- **Web hosting (HTTP/HTTPS)**  
- **Email (SMTP & POP3)**  
- **OSPF dynamic routing**  

---

## 📂 Project Structure
networks-packettracer-project/  
├── topology.pkt              — Cisco Packet Tracer topology file  
├── Report.pdf                — Full project report with theory, configs, results  
└── README.md                 — Project documentation  

---

## ⚙️ Features
- **Subnetting & IP Addressing:** Designed from `110.54.8.0/23` block → divided into multiple subnets (/26, /27, /30).  
- **Dynamic Routing (OSPF):** Configured across routers (Areas 0–4) for scalability.  
- **DHCP:** Configured in University & Street networks for dynamic IP allocation.  
- **DNS:** Resolves `www.coe.birzeit.edu` and `mail.coe.birzeit.edu`.  
- **Web Server:** Hosts a faculty web page with HTML and images.  
- **Mail Server:** Supports SMTP (sending) and POP3 (receiving), with user accounts for each subnet.  
- **Wireless Access Point:** Provides Wi-Fi for NET1-B (University wireless).  

---

## 📊 Results
- **Connectivity Tests:** Successful ping and tracert across all networks.  
- **Web Server:** Accessible from University, Street, and Home devices (`http://www.coe.birzeit.edu`).  
- **Email:** Verified sending/receiving between users in University and Home networks.  
- **DHCP:** Automatic IP assignment for laptops and smartphones.  
- **OSPF:** Correct route advertisement and convergence across routers.  

---

## ⚠️ Issues & Limitations
- DHCP relay needed on Router0 for wireless clients.  
- NET2 subnet split into two /28s due to server interface limitations.  
- Packet Tracer limitations: some pings failed despite correct configs.  
- Time constraints (solo project) limited advanced testing.  

---

## 🚀 How to Run
1. Open `topology.pkt` in Cisco Packet Tracer.  
2. Verify router configs (OSPF, static IPs, DHCP relay).  
3. Test connectivity with:  
   - `ping` and `tracert` between devices.  
   - Access `http://www.coe.birzeit.edu` from browsers.  
   - Send/receive emails using configured Mail server accounts.  

---

## 👩‍🎓 Author
**Rawand Radi**  
Faculty of Engineering and Technology – Birzeit University  
Course: Computer Networks (ENCS3320)  
Instructor: Dr. Ibrahem Nemir  
Date: June 18, 2025
