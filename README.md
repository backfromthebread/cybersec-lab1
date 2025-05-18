# cybersec-lab1

My first custom attack lab: Node.js web server on Windows 10, scanned and accessed from Kali Linux 💻  
📘 Lab 01 – Node.js Web Server Recon  
📅 Date: May 18, 2025  
🎯 Goal: Set up a Node.js server on Windows 10 and access it from Kali Linux for scanning, interception, and replay.

---

## 🧱 Setup

**Target Machine:** Windows 10 (VMware)  
**Attacker Machine:** Kali Linux (VMware)  
**Networking:** NAT (same subnet)

---

## 🛠️ Tools Used

- Node.js + Express  
- Kali Linux  
- Nmap  
- Firefox  
- curl  
- BurpSuite Community Edition

---

## 🔥 What I Did

- Installed Node.js on Windows 10  
- Created a basic Express server on port 3000  
- Disabled Windows Firewall for lab purposes  
- Found target IP using `ipconfig`  
- Accessed the server from Kali via browser + `curl`  
- Ran `nmap` to detect open port  
- Verified traffic between machines  
- Submitted login form from Kali → captured by BurpSuite  
- Forwarded POST request in Burp  
- Sent request to **Repeater**, modified credentials, and re-sent  
- Verified captured data was logged in Node.js console

---

## 🔍 Interception + Replay (BurpSuite)

- Set Firefox proxy to `127.0.0.1:8080`  
- Opened BurpSuite → Intercept ON  
- Visited `http://192.168.113.130:3000/login` on Kali  
- Filled form: `admin / 123456`  
- BurpSuite intercepted POST request with raw form data  
- Forwarded the intercepted request  
- Sent the request to **Repeater**  
- Changed form values manually to test different credentials  
- Replayed and confirmed modified credentials were accepted by backend

---

## 🧠 Key Takeaways

- First successful interaction between attacker and target  
- Learned how Express serves data and how Kali can access it  
- Practiced HTTP interception and replay with BurpSuite  
- Foundation for future attacks (login forms, brute-force, fuzzing)


![{D7F90C6D-BF2E-4A3D-BB69-D79634A067EB}](https://github.com/user-attachments/assets/517224e7-8c6d-41a9-a06b-104f0b897319)

![{3E272271-9EC3-47D4-AF9C-6381F1466130}](https://github.com/user-attachments/assets/1403a46a-6c1c-4408-85f5-a33dd04083c4)

![{3420D8CA-7C55-4D53-BC8B-231D3A30FEE2}](https://github.com/user-attachments/assets/d7644abe-22f5-445e-8216-d834f2054cea)

