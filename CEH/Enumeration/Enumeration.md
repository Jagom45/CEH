# Enumeration

# Perform NetBIOS Enumeration
- Use Windows command-line utilities like nbtstat and net use to enumerate target machines and gather data about NetBIOS names, shares, and policies.

# Use SnmpWalk to enumerate network resources such as routers, ARP tables, and traffic statistics. Explore SNMP versions 1 and 2c to collect information about network devices and configurations
- Use SnmpWalk to enumerate network resources such as routers, ARP tables, and traffic statistics. Explore SNMP versions 1 and 2c to collect information about network devices and configurations

# Perform LDAP Enumeration
-Use Active Directory Explorer (AD Explorer) to gather information about directory listings, user accounts, and network components, and explore how directory services can reveal sensitive information

# Perform NFS Enumeration
-Utilize RPCScan and SuperEnum to identify NFS shares, directories, and connected clients, which could expose shared files and other network resources for exploitation.

# Perform DNS Enumeration
- Perform DNS zone transfer using tools like dig and nslookup to extract DNS server information, hostnames, and machine names, while testing for vulnerabilities in the DNS configuration

# Perform SMTP Enumeration
- Use Nmap scripts to enumerate the SMTP server running on the target machine. Identify valid email users and test for open SMTP relays to uncover potential vulnerabilities

# Perform Enumeration using Global Network Inventory
-Use the Global Network Inventory tool to gather detailed information about the target network, including services, user groups, shares, and installed software

# Perform Enumeration using AI
- Leverage AI-powered enumeration using ShellGPT to automate tasks like NetBIOS, SNMP, and DNS enumeration, and streamline the process of gathering detailed data on the target network

# Module 04: Enumeration

Objective
The objective of the lab is to extract information about the target organization that includes, but is not limited to:

Machine names, their OSes, services, and ports
Network resources
Usernames and user groups
Lists of shares on individual hosts on the network
Policies and passwords
Routing tables
Audit and service settings
SNMP and FQDN details
Overview of Enumeration
Enumeration creates an active connection with the system and performs directed queries to gain more information about the target. It extracts lists of computers, usernames, user groups, ports, OSes, machine names, network resources, and services using various techniques. Enumeration techniques are conducted in an intranet environment.




# Lab 1: Perform NetBIOS Enumeration


Lab Objectives

Perform NetBIOS enumeration using Windows command-line utilities
Overview of NetBIOS Enumeration

NetBIOS stands for Network Basic Input Output System. Windows uses NetBIOS for file and printer sharing. A NetBIOS name is a unique computer name assigned to Windows systems, comprising a 16-character ASCII string that identifies the network device over TCP/IP. The first 15 characters are used for the device name, and the 16th is reserved for the service or name record type.

The NetBIOS service is easily targeted, as it is simple to exploit and runs on Windows systems even when not in use. NetBIOS enumeration allows attackers to read or write to a remote computer system (depending on the availability of shares) or launch a denial of service (DoS) attack.







Common NetBIOS suffixes and types
Suffix

Type

Description

<00>

UNIQUE

Workstation service name

<00>

GROUP

Domain or workgroup name

<20>

UNIQUE

File Server Service

<1E>

GROUP

Browser service elections

<1D>

UNIQUE

Local master browser

<1B>

UNIQUE

Domain master browser

<1C>

GROUP

Domain controllers

<01>

GROUP

Master Browser

Remember the difference
UNIQUE: Identifies one individual computer or service.

GROUP: Identifies a group of computers or services.

Important: The same suffix can appear as either UNIQUE or GROUP depending on its purpose. For example, <00> can be either UNIQUE (computer name) or GROUP (workgroup name).

For studying, remember this common sequence:

<00> UNIQUE

<00> GROUP

<20> UNIQUE

<1E> GROUP

<1D> UNIQUE

<01> GROUP

The exact entries and order can vary depending on the computer's configuration.

# Lab 2: Perform SNMP Enumeration

- Lab Objectives
Perform SNMP enumeration using SnmpWalk

Overview of SNMP Enumeration

SNMP (Simple Network Management Protocol) is an application layer protocol that runs on UDP (User Datagram Protocol) and maintains and manages routers, hubs, and switches on an IP network. SNMP agents run on networking devices on Windows and UNIX networks.

SNMP enumeration uses SNMP to create a list of the user accounts and devices on a target computer. SNMP employs two types of software components for communication: the SNMP agent and SNMP management station. The SNMP agent is located on the networking device, and the SNMP management station communicates with the agent.

# Lab 3: Perform LDAP Enumeration

 - Lab Objectives
Perform LDAP enumeration using Active Directory Explorer (AD Explorer)

- Overview of LDAP Enumeration

LDAP (Lightweight Directory Access Protocol) is an Internet protocol for accessing distributed directory services over a network. LDAP uses DNS (Domain Name System) for quick lookups and fast resolution of queries. A client starts an LDAP session by connecting to a DSA (Directory System Agent), typically on TCP port 389, and sends an operation request to the DSA, which then responds. BER (Basic Encoding Rules) is used to transmit information between the client and the server. One can anonymously query the LDAP service for sensitive information such as usernames, addresses, departmental details, and server names.****

# Lab 4: Perform NFS Enumeration

- Lab Objectives
Perform NFS enumeration using RPCScan and SuperEnum

- Overview of NFS Enumeration
NFS (Network File System) is a type of file system that enables computer users to access, view, store, and update files over a remote server. This remote data can be accessed by the client computer in the same way that it is accessed on the local system.

# Lab 5: Perform DNS Enumeration

- Lab Objectives

Perform DNS enumeration using zone transfer
- Overview of DNS Enumeration

DNS enumeration techniques are used to obtain information about the DNS servers and network infrastructure of the target organization. DNS enumeration can be performed using the following techniques:

Zone transfer


# Lab 6: Perform SMTP Enumeration
- Lab Objectives

Perform SMTP enumeration using Nmap

- Overview of SMTP Enumeration

The Simple Mail Transfer Protocol (SMTP) is an internet standard based communication protocol for electronic mail transmission. Mail systems commonly use SMTP with POP3 and IMAP, which enable users to save messages in the server mailbox and download them from the server when necessary. SMTP uses mail exchange (MX) servers to direct mail via DNS. It runs on TCP port 25, 2525, or 587.

# Lab 7: Perform Enumeration using Various Enumeration Tools

- Lab Objectives

Enumerate information using Global Network Inventory
- Overview of Enumeration Tools

To recap what you have learned so far, enumeration tools are used to collect detailed information about target systems in order to exploit them. The information collected by these enumeration tools includes data on the NetBIOS service, usernames and domain names, shared folders, the network (such as ARP tables, routing tables,traffic, etc.), user accounts, directory services, etc.

# Lab 8: Perform Enumeration using AI
Lab Objectives
-Perform Enumeration using ShellGPT

- Overview of Enumeration using AI

Artificial Intelligence (AI) can significantly enhance the enumeration process by automating tasks, analyzing large datasets, and identifying patterns that might be missed by traditional tools. AI can streamline the enumeration process, making it faster, more efficient, and more accurate.
























