# Elevate_Lab_CYBER_-SECURITY_INTERNSHIP
DAY-1

#  Nmap Network Scanning Task

## Task Overview
This task demonstrates basic network reconnaissance using **Nmap** on a local network.

## Steps Performed
1. Installed Nmap on Kali Linux.
2. Identified local IP range .
3. Performed a TCP SYN scan:
   sudo nmap -sS 192.168.0.0/24
Saved scan results:

As .txt: -oN results.txt

![image](https://github.com/user-attachments/assets/a11e6930-1d02-435e-83fb-99f292a762bc)


 Day-2:
 **Collect Email Sample**  
   Obtained a sample email for analysis.

2. **Verify Sender**  
   Checked sender's email (`kinaxis+autoreply@talent.icims.com`) — found to be authentic.

3. **Analyze Headers**  
   Used email headers to verify SPF, IP, and routing — no spoofing or discrepancies found.

4. **Inspect Links & Attachments**  
   - No attachments.
   - All URLs from trusted domains (`icims.com`, `kinaxis.com`).

5. **Check Language & Tone**  
   No urgency, threats, or manipulation tactics. Professional tone maintained.

6. **Compare URLs**  
   Hover links matched actual URLs — no redirection or mismatches.

7. **Grammar & Spelling Check**  
   No errors found; well-written content.

#DAY-3
This task involves performing a vulnerability scan on my own Linux system using Nessus Essentials to identify potential security issues.

Installed and configured Nessus Essentials on Kali Linux.

Set the scan target as 127.0.0.1 (localhost).

Launched a full system vulnerability scan.

Waited for the scan to complete (~45 minutes).

Reviewed the report and noted vulnerabilities by severity.

Researched and documented simple fixes for the most critical issues.

Captured screenshots of key scan results and exported the report in csv format.

Day-4
 Task 4: Firewall Setup using UFW on Kali Linux
 Objective
Configure and test firewall rules using UFW (Uncomplicated Firewall) to understand traffic filtering and improve basic firewall skills.

 Tools Used
OS: Kali Linux

Firewall Tool: UFW

 Steps Summary
Installed and enabled UFW:


sudo apt install ufw -y  
sudo ufw enable
Checked existing rules:

sudo ufw status verbose
Blocked Telnet (port 23):

sudo ufw deny 23
Tested port block using Telnet and Netcat.

Allowed SSH (port 22):
sudo ufw allow 22
Removed Telnet block rule:


sudo ufw delete [22]

Day-5
Wireshark Packet Capture Task
 Objective
Capture and analyze network traffic using Wireshark to identify common protocols and understand packet-level communication.

 Tools Used
OS: Kali Linux

Tool: Wireshark

 Task Summary
Installed Wireshark using APT.

Started live capture on the active network interface.

Generated traffic by browsing a website and pinging a server.

Stopped the capture after one minute.

Applied filters: dns, http, tcp.

Identified protocols: DNS, TCP, HTTP.

Exported capture as my_capture.pcap.

