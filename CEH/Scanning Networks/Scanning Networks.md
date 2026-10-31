# Module 03: Scanning Networks
- 

# Perform Host Discovery using Nmap
- Use Nmap to discover active hosts in the target network. Apply various host discovery techniques like ARP ping scan, UDP ping scan, ICMP ECHO ping scan, and more to locate live systems

# Perform Port and Service Discovery using Nmap
- Discover open ports and running services using various Nmap scanning techniques, such as TCP connect scan, Xmas scan, UDP scan, and ACK flag probe scan, to identify potential vulnerabilities

# Perform OS Discovery using Nmap Script Engine (NSE)
- Perform OS fingerprinting using Nmap's aggressive scan and OS discovery techniques to identify the operating system running on target machines, and extract valuable details about the target's system.

# Scan beyond IDS/Firewall using various Evasion Techniques
- Learn how to bypass IDS and firewall protections by utilizing techniques such as packet fragmentation, source port manipulation, IP address decoy, and MAC address spoofing to scan target systems undetected.

# Scan a Target Network using Metasploit
- Use Metasploit Framework to scan a network, identify open ports, services running, and gather information about the operating systems on target systems within the network.

# Perform Network Scanning using AI (ShellGPT)
- Leverage AI-powered tools like ShellGPT to automate the network scanning process, including host discovery, port scanning, service enumeration, and OS fingerprinting, and use AI for faster analysis of vulnerabilities.



# Module 03: Scanning Networks

- The objective of this lab is to conduct network scanning, port scanning, analyzing the network vulnerabilities, etc.
- Network scans are needed to:
- Check live systems and open ports
- Identify services running in live systems
- Perform banner grabbing/OS fingerprinting
- Identify network vulnerabilities


# Lab 1: Perform Host Discovery
- Perform host discovery using Nmap

- Host discovery is considered the primary task in the network scanning process. It is used to discover the active/live hosts in a network. It provides an accurate status of the systems in the network, which, in turn, reduces the time spent on scanning every port on every system in a sea of IP addresses in order to identify whether the target host is up.

The following are examples of host discovery techniques:

ARP ping scan
UDP ping scan
ICMP ping scan (ICMP ECHO ping, ICMP timestamp, ping ICMP, and address mask ping)
TCP ping scan (TCP SYN ping and TCP ACK ping)
IP protocol ping scan

# Lab 2: Perform Port and Service Discovery
- Explore various network scanning techniques using Nmap
Overview of Port and Servi

- Port scanning techniques are categorized according to the type of protocol used for communication within the network.

TCP Scanning
Open TCP scanning methods (TCP connect/full open scan)
Stealth TCP scanning methods (Half-open Scan, Inverse TCP Flag Scan, ACK flag probe scan, third party and spoofed TCP scanning methods)
UDP Scanning
SCTP Scanning
SCTP INIT Scanning
SCTP COOKIE/ECHO Scanning
SSDP and List Scanning
IPv6 Scanning

# Lab 3: Perform OS Discovery
- Perform OS discovery using Nmap Script Engine (NSE)

- Banner grabbing, or OS fingerprinting, is a method used to determine the OS that is running on a remote target system.

There are two types of OS discovery or banner grabbing techniques:

Active Banner Grabbing Specially crafted packets are sent to the remote OS, and the responses are noted, which are then compared with a database to determine the OS. Responses from different OSes vary, because of differences in the TCP/IP stack implementation.

Passive Banner Grabbing This depends on the differential implementation of the stack and the various ways an OS responds to packets. Passive banner grabbing includes banner grabbing from error messages, sniffing the network traffic, and banner grabbing from page extensions.

Parameters such as TTL and TCP window size in the IP header of the first packet in a TCP session plays an important role in identifying the OS running on the target machine. The TTL field determines the maximum time a packet can remain in a network, and the TCP window size determines the length of the packet reported. These values differ for different OSes: you can refer to the following table to learn the TTL values and TCP window size associated with various OSes.


# Lab 4: Scan beyond IDS and Firewall
- Scan beyond IDS/firewall using various evasion techniques

- Overview of Scanning beyond IDS and Firewall

An Intrusion Detection System (IDS) and firewall are the security mechanisms intended to prevent an unauthorized person from accessing a network. However, even IDSs and firewalls have some security limitations. Firewalls and IDSs intend to avoid malicious traffic (packets) from entering into a network, but certain techniques can be used to send intended packets to the target and evade IDSs/firewalls.

Techniques to evade IDS/firewall:

Packet Fragmentation: Send fragmented probe packets to the intended target, which re-assembles it after receiving all the fragments
Source Routing: Specifies the routing path for the malformed packet to reach the intended target
Source Port Manipulation: Manipulate the actual source port with the common source port to evade IDS/firewall
IP Address Decoy: Generate or manually specify IP addresses of the decoys so that the IDS/firewall cannot determine the actual IP address
IP Address Spoofing: Change source IP addresses so that the attack appears to be coming in as someone else
Creating Custom Packets: Send custom packets to scan the intended target beyond the firewalls
Randomizing Host Order: Scan the number of hosts in the target network in a random order to scan the intended target that is lying beyond the firewall
Sending Bad Checksums: Send the packets with bad or bogus TCP/UDP checksums to the intended target
Proxy Servers: Use a chain of proxy servers to hide the actual source of a scan and evade certain IDS/firewall restrictions
Anonymizers: Use anonymizers that allow them to bypass Internet censors and evade certain IDS and firewall rules

# Lab 5: Perform Network Scanning using Various Scanning Tools
- Scan a target network using Metasploit

Overview of Network Scanning Tools

Scanning tools are used to scan and identify live hosts, open ports, running services on a target network, location-info, NetBIOS info, and information about all TCP/IP and UDP open ports. Information obtained from these tools will assist an ethical hacker in creating the profile of the target organization and to scan the network for open ports of the devices connected.

# Lab 6: Perform Network Scanning using AI
- Scan a target using ShellGPT

- Overview of Network Scanning using AI

Network scanning using AI enhances cybersecurity by automating the detection of vulnerabilities and threats. AI-driven tools analyze network traffic, identify anomalies, and predict potential attacks with high accuracy, providing proactive defense mechanisms and reducing response times for cybersecurity teams.








