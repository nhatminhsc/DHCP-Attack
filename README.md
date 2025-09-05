# DHCP Attacks: Starvation & Spoofing

## 📌 Overview
This project demonstrates two common attacks against the **DHCP protocol** in a virtualized lab environment:  

- **DHCP Starvation**: Exhausting the IP pool of the legitimate DHCP server, causing denial of service for valid clients.  
- **DHCP Spoofing**: Running a rogue DHCP server to assign fake IP, gateway, and DNS information to clients, enabling traffic redirection and potential Man-in-the-Middle (MITM) scenarios.  

## 🧪 Lab Environment
The lab is built using **VMware Workstation** with the following virtual machines:  
- **Windows Server 2019** → DHCP server  
- **Windows 10** → DHCP client  
- **Kali Linux** → attacker machine  
- Network adapter: **Host-only (VMnet1)**  

## 🚀 Results
- Successfully performed **DHCP Starvation** using the tool [DHCPig](https://github.com/kamorin/DHCPig).  
- Successfully launched a **DHCP Spoofing attack**, where the Kali attacker provided rogue DHCP responses and assigned clients an IP, gateway, and DNS.  

## 🔮 Future Work
Possible improvements and extensions of this project:  
- **DNS Spoofing**: Redirecting domain queries to a fake server.  
- **MITM attack**: Using Kali as a router with IP forwarding and packet inspection.  
- **Phishing demo**: Hosting a fake web server for redirected clients.  
- **Defense mechanisms**: Exploring features like DHCP Snooping, IP Source Guard, and Dynamic ARP Inspection.  

## 📖 Full Write-up
The detailed step-by-step lab write-up with screenshots is available here:  
👉 [HackMD Write-up (Vietnamese Only)](https://hackmd.io/@FLFwOI7sTB6F-qAm07OXLQ/HyBlMJI9lg)

---
