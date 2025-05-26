# task
scanning the network with nmap

### Scanning the local network for open ports### 
1.first install the nmap on you machine or use kali linux nmap comes in-built
2. find the local ip address with the command ip a or ifconfig ex:192.168.1.15
3. use the nmap command: nmap -sS <ip address/range> ex:192.168.1.15/24
4. you will get the output 

![Image](https://github.com/user-attachments/assets/9f7724f8-7125-4902-8806-e9a146356bd2)

### . port details and  uses ### 

 135: TCP port 135 is used for the Microsoft Remote Procedure Call (RPC) service, which allows communication between different processes on a network. It's also used for the MSRPC endpoint mapper, which helps determine which ports other services are running on. 
139: TCP port 139 is primarily used by NetBIOS over TCP/IP, which is a protocol used for network communications, particularly for file and printer sharing. 
445: TCP port 445 is also used by the SMB protocol for file and printer sharing. 

5. security risk: 
SMB Vulnerabilities:
Port 445 and the SMB protocol have been exploited in past attacks like WannaCry, where a vulnerability in SMB allowed attackers to spread ransomware across networks. 
Exploitation of RPC:
Port 135 can be exploited for remote code execution and other malicious activities. 
Brute-Force Attacks:
Brute-force attacks on these ports can be used to gain unauthorized access to systems. 
Open Ports:
Leaving these ports open can expose systems to various cyber threats, including malware, ransomware, and other attacks

