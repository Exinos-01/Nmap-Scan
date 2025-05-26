# Nmap-Scan 
# Cybersecurity Internship – Task 1

## Task: Scan Your Local Network for Open Ports

###  Objective:
Use **Nmap** to perform a **TCP SYN scan** on your local network, identify open ports, and understand basic network exposure.
##  Tools Used:
- [Nmap](https://nmap.org) – for scanning

## My Local IP Range:
I found my local IP address using `ipconfig` and determined my network range as:
192.168.1.0/24 yaml

##Nmap Command Used:

nmap -sS 192.168.1.0/24
This performs a TCP SYN scan across all devices in my local subnet.

Scan Results Summary:
Example Device:
IP: 192.168.1.8

Open Ports:
Port 21: FTP

Port 22: SSH

Port 80: HTTP


Risk Analysis:
Port 22 (SSH):

If not secured with strong passwords or disabled root login, could be vulnerable to brute force attacks.

Port 80 (HTTP):

If a web server is running, it could leak information or be vulnerable to attacks (e.g., directory traversal).

Recommendation:

Close unused ports via firewall or service management.

Use firewalls to restrict access.

Use secure configurations (disable default credentials, update software).

Learnings:
Understood how to find my IP range and scan devices on the network.

Learned about common open ports and their associated risks.

Got hands-on experience with Nmap and network reconnaissance.

📎 Files Included:
scan_results.txt: Raw output of the Nmap scan
