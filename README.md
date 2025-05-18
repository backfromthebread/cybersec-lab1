# cybersec-lab1
My first custom attack lab: Node.js web server on Windows 10, scanned and accessed from Kali Linux
💻 Lab 01 – Node.js Web Server Recon
Date: May 18, 2025
Goal: Set up a Node.js server on Windows 10 and access it from Kali Linux for scanning and recon.

🧱 Setup

Target Machine: Windows 10 (VMware)

Attacker Machine: Kali Linux (VMware)

Networking: NAT (same subnet)

🔧 Tools Used
Node.js + Express

Kali Linux

Nmap

Firefox

curl


🔥 What I Did

Installed Node.js on Windows 10

Created a basic Express server on port 3000

Disabled Windows Firewall for lab purposes

Found target IP using ipconfig

Accessed the server from Kali via browser + curl

Ran nmap to detect open port

Verified traffic between machines


🧠 Key Takeaways

First successful interaction between attacker and target

Learned how Express serves data and how Kali can access it

Foundation for future attacks (login forms, BurpSuite, fuzzing)


![{D7F90C6D-BF2E-4A3D-BB69-D79634A067EB}](https://github.com/user-attachments/assets/517224e7-8c6d-41a9-a06b-104f0b897319)
![{3E272271-9EC3-47D4-AF9C-6381F1466130}](https://github.com/user-attachments/assets/1403a46a-6c1c-4408-85f5-a33dd04083c4)
