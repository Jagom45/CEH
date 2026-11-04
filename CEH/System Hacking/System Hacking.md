# System Hacking
- Perform active online attack to crack the system's password using Responder
- Use Responder to capture NTLMv2 hashes from a target system and crack the password using John the Ripper. This will demonstrate the vulnerability of poorly secured network protocols and the ease of capturing user credentials

- Gain access to a remote system using Reverse Shell Generator
- Use Reverse Shell Generator to create and deploy a payload that will establish a remote connection to the target system. This task simulates how attackers gain control over remote systems using reverse shells.

- Perform buffer overflow attack to gain to a remote system
- Execute a buffer overflow attack on a vulnerable service to gain unauthorized access. This task will cover the exploitation of memory management vulnerabilities to execute arbitrary code on the target machine.

- Escalate privileges by bypassing UAC and exploiting Sticky Keys
- Perform privilege escalation by exploiting Windows UAC and Sticky Keys features. This task demonstrates how attackers can elevate privileges and gain administrative access by exploiting OS misconfigurations.

- Maintain remote access and hide malicious activities
- Use Spyrix to monitor user activities and maintain persistence on the target system by modifying registry run keys. This task covers techniques to ensure prolonged access to a compromised system without detection.

- Perform system hacking using ShellGPT
- Leverage ShellGPT to automate various system hacking tasks, including payload generation and vulnerability scanning. ShellGPT can enhance penetration testing efforts by providing dynamic, AI-driven strategies for exploitation and analysis.

Module 06: System Hacking
- Objective
The objective of this task is to monitor a target system remotely and perform other tasks that include, but are not limited to:

Bypassing access controls to gain access to the system (such as password cracking and vulnerability exploitation)
Acquiring the rights of another user or an admin (privilege escalation)
Creating and maintaining remote access to the system (executing applications such as trojans, spyware, backdoors, and keyloggers)
Hiding malicious activities and data theft (executing applications such as Rootkits, steganography, etc.)
Hiding the evidence of compromise (clearing logs)

- Overview of System Hacking
In preparation for hacking a system, you must follow a certain methodology. You need to first obtain information during the footprinting, scanning, enumeration, and vulnerability analysis phases, which can be used to exploit the target system.

There are four steps in the system hacking:

Gaining Access: Use techniques such as cracking passwords and exploiting vulnerabilities to gain access to the target system

Escalating Privileges: Exploit known vulnerabilities existing in OSes and software applications to escalate privileges

Maintaining Access: Maintain high levels of access to perform malicious activities such as executing malicious applications and stealing, hiding, or tampering with sensitive system files

Clearing Logs: Avoid recognition by legitimate system users and remain undetected by wiping out the entries corresponding to malicious activities in the system logs, thus avoiding detection.


# Lab 1: Gain Access to the System

- Lab Objectives

Perform active online attack to crack the system's password using Responder
Gain access to a remote system using Reverse Shell Generator
Perform buffer overflow attack to gain access to a remote system

- Overview of Gaining Access

The previous phases of hacking such as footprinting and reconnaissance, scanning, enumeration, and vulnerability assessment help identify security loopholes and vulnerabilities that exist in the target organizational IT assets. You can use this information to gain access to the target organizational systems. You can use various techniques such as passwords cracking and vulnerability exploitation to gain access to the target system.

# Task 2: Gain Access to a Remote System using Reverse Shell Generator


# Task 3: Perform Buffer Overflow Attack to Gain Access to a Remote System

# Lab 2: Perform Privilege Escalation to Gain Higher Privileges

- Lab Objectives

Escalate privileges by bypassing UAC and exploiting Sticky Keys
Overview of Privilege Escalation

Privileges are a security role assigned to users for specific programs, features, OSes, functions, files, or codes. They limit access by type of user. Privilege escalation is required when you want to access system resources that you are not authorized to access. It takes place in two forms: vertical privilege escalation and horizontal privilege escalation.

Horizontal Privilege Escalation: An unauthorized user tries to access the resources, functions, and other privileges that belong to an authorized user who has similar access permissions

Vertical Privilege Escalation: An unauthorized user tries to gain access to the resources and functions of a user with higher privileges such as an application or site administrator

# Lab 3: Maintain Remote Access and Hide Malicious Activities

- Lab Objectives

User system monitoring and surveillance using ReFOG
Maintain persistence by modifying registry run keys
Overview of Remote Access and Hiding Malicious Activities

Remote Access: Remote code execution techniques are often performed after initially compromising a system and further expanding access to remote systems present on the target network.

Discussed below are some of the remote code execution techniques:

Exploitation for client execution
Scheduled task
Service execution

# Lab 4: Clear Logs to Hide the Evidence of Compromise

- Lab Objectives

Clear Windows machine logs using various utilities
Clear Linux machine logs using the BASH shell
Overview of Clearing Logs

To remain undetected, the intruders need to erase all evidence of security compromise from the system. To achieve this, they might modify or delete logs in the system using certain log-wiping utilities, thus removing all evidence of their presence.

Various techniques used to clear the evidence of security compromise are as follow:

Disable Auditing: Disable the auditing features of the target system
Clearing Logs: Clears and deletes the system log entries corresponding to security compromise activities
Manipulating Logs: Manipulate logs in such a way that an intruder will not be caught in illegal actions
Covering Tracks on the Network: Use techniques such as reverse HTTP shells, reverse ICMP tunnels, DNS tunneling, and TCP parameters to cover tracks on the network.
Covering Tracks on the OS: Use NTFS streams to hide and cover malicious files in the target system
Deleting Files: Use command-line tools such as Cipher.exe to delete the data and prevent its future recovery
Disabling Windows Functionality: Disable Windows functionality such as last access timestamp, Hibernation, virtual memory, and system restore points to cover tracks

# Lab 5: Perform Active Directory (AD) Attacks Using Various Tools

- Lab Objectives

Perform Initial Scans to Obtain Domain Controller IP and Domain Name
Perform AS-REP Roasting attack
Spray cracked password into network using CrackMapExec
Perform post-enumeration using PowerView
Perform Attack on MSSQL service
Perform privilege escalation
Perform Kerberoasting Attack
Overview of AD Attacks

AD attacks involve exploiting vulnerabilities in the AD to gain unauthorized access, escalate privileges, and steal sensitive data. Techniques include password cracking, Kerberos attacks, and exploiting misconfigurations. As ethical hackers, you can use these methods to test defenses, identify weaknesses, and enhance security for organizations' network infrastructures.

# Lab 6: Perform System Hacking using AI
 
 - Lab Objectives

Perform system hacking using ShellGPT
Overview of System Hacking using AI

System hacking using AI leverages advanced algorithms to identify and exploit vulnerabilities efficiently. AI tools automate tasks like password cracking, vulnerability scanning, and social engineering, enhancing the capabilities of ethical hackers. This approach improves the accuracy and speed of penetration testing, ensuring robust security assessments and effective mitigation strategies. 


