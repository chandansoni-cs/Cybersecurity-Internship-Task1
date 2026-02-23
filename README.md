***Objective:- Foundation & Environment Setup***

The objective of this task is to develop a strong foundation in cybersecurity concepts, networking principles, and cryptography while setting up a professional virtual lab environment for ethical hacking practice.

This task focuses on understanding the CIA Triad, common cyber threats, Linux fundamentals, networking basics, and encryption concepts. It also involves configuring a virtual environment using Kali Linux and a vulnerable target machine to perform controlled security testing.

**Cyber Security :-**

***1.CIA Triad in Cyber Security***

Introduction:-

The CIA Triad is a fundamental concept in Cyber Security.

CIA stands for:

C – Confidentiality

I – Integrity

A – Availability

It defines the three core principles that ensure information security in any system.

**Confidentiality**

 Meaning:

  Confidentiality ensures that sensitive information is accessible only to authorized users.

 Goal:

  Prevent unauthorized access to data.

 Examples:

  Password protection

  OTP authentication

  Encryption (AES, RSA)

  Biometric authentication

 Real Life Example:

  When you log in to your Gmail account, only you should access your emails.

 Techniques Used:

  Encryption

  Access Control

  Multi-Factor Authentication (MFA)

  Firewalls

**Integrity**

Meaning:

Integrity ensures that data remains accurate and unchanged unless modified by authorized users.

Goal:

Prevent unauthorized data modification.

Examples:

Hashing (SHA-256)

Digital Signatures

Checksums

Real Life Example:

If you transfer ₹5000 through PhonePe, the amount should not change during transmission.

Techniques Used:

Hash Functions

Data Validation

Version Control

Digital Signatures

**Availability**

Meaning:

Availability ensures that data and systems are accessible when needed.

Goal:

Ensure system uptime and reliability.

Examples:

Backup systems

Cloud storage

Load balancing

DDoS protection

Real Life Example:

Banking websites should be available 24/7.

Techniques Used:

Redundancy

Regular Backups

Disaster Recovery Plans

Server Clustering

Why CIA Triad is Important?

Without CIA Triad:

-Data can be stolen

-Data can be modified

-Systems can go down 

With CIA Triad:

-Data is secure 

-Data is accurate 

-Systems are reliable 

How CIA Triad Works Together

All three principles must work together:

1. If data is confidential but not available → Useless

2. If data is available but not confidential → Dangerous

3. If data is confidential but not accurate → Unreliable

Security is balanced only when all three are maintained.

**Conclusion**

The CIA Triad is the foundation of Information Security.
Every security mechanism is designed to protect at least one of these three principles.

Understanding CIA helps in:

Ethical Hacking

Network Security

System Administration

Cloud Security


***2.Common Cyber Threats***

Cyber threats are malicious activities designed to steal, damage, or disrupt data, networks, and systems. Understanding these threats is essential for cybersecurity.

**Phishing**

Definition:-  Phishing is a cyber attack in which attackers send fake emails, messages, or create fraudulent websites to trick users into revealing sensitive information.

Target:-

Passwords

Credit/Debit card details

OTPs

Personal information

Example:-

An attacker sends an email pretending to be from a bank asking the user to verify account details through a fake link.

Prevention:-

1.Avoid clicking suspicious links

2.Verify sender email addresses

3.Enable Multi-Factor Authentication (MFA)


**Malware**

Definition:- Malware (Malicious Software) is software intentionally designed to damage systems or gain unauthorized access.

Types:- Virus,Worm,Trojan,Spyware

Example:-

Downloading pirated software that secretly installs harmful code on the system.

Prevention:-

1.Install and update antivirus software

2.Download software from trusted sources only

3.Keep operating systems updated

**DDoS (Distributed Denial of Service)**

Definition:- A DDoS attack overwhelms a server or network with massive traffic, making services unavailable to legitimate users.

Goal:-  Disrupt services and cause downtime.

Example:-

Attackers send large volumes of fake traffic to crash a website during peak hours.

Prevention:-

1.Use firewalls and intrusion detection systems

2.Implement load balancing

3.Use DDoS protection services

**SQL Injection**

Definition:- SQL Injection is an attack where malicious SQL queries are inserted into input fields to manipulate or access a database.

Target:-

User credentials

Sensitive database records

Administrative access

Example:-

An attacker enters malicious SQL code into a login form to bypass authentication.

Prevention:-

1.Use parameterized queries

2.Implement input validation

3.Use prepared statements

**Brute Force Attack**

Definition:- A brute force attack attempts to gain access by systematically trying multiple password combinations.

Target:-

User accounts

Admin panels

Example:-

Automated tools try thousands of password combinations to access an account.

Prevention:-

1.Use strong passwords

2.Enable account lockout mechanisms

3.Implement Two-Factor Authentication (2FA)

**Ransomware**

Definition:- Ransomware is a type of malware that encrypts a victim’s data and demands payment for decryption.

Goal:- Financial extortion.

Example:-

An organization’s files are encrypted, and attackers demand cryptocurrency to restore access.

Prevention:-

1.Maintain regular backups

2.Avoid opening unknown attachments

3.Keep software and systems updated



***3.Attack Vectors***

An attack vector is the method or pathway used by attackers to gain unauthorized access to a system, network, or data. Understanding attack vectors helps organizations strengthen their security defenses.

**Social Engineering**

Definition:- Social engineering is a technique where attackers manipulate people into revealing confidential information or performing actions that compromise security.

Common Techniques:-

Phishing emails

Pretexting (fake identity or scenario)

Baiting (offering something attractive to gain access)

Tailgating (unauthorized physical access)

Example:- An attacker calls an employee pretending to be from the IT department and asks for login credentials.

Prevention:-

 1.Security awareness training

 2.Verification of identity before sharing information

 3.Strong access control policies

**Wireless Attacks**

Definition:- Wireless attacks target Wi-Fi networks and wireless communication systems to intercept or manipulate data.

Common Types:-

Evil Twin Attack (fake Wi-Fi access point)

Man-in-the-Middle (MitM) attack

Wi-Fi password cracking

Packet sniffing

Example:- An attacker sets up a fake public Wi-Fi network to capture users’ login credentials.

Prevention:-

 1.Use strong Wi-Fi encryption (WPA3)

 2.Avoid public Wi-Fi for sensitive transactions

 3.Use VPN for secure communication

 4.Disable automatic Wi-Fi connections

**Insider Threats**

Definition:- An insider threat occurs when a person within an organization (employee, contractor, or partner) misuses their authorized access to harm the organization.

Types:-

Malicious insider (intentional harm)

Negligent insider (careless behavior)

Compromised insider (account hijacked by attackers)

Example:- An employee leaks confidential company data to competitors.

Prevention:-

 1.Role-based access control

 2.Monitoring and logging user activities

 3.Regular security audits

 4.Employee background verification

Conclusion:-

Attack vectors represent the entry points used by cybercriminals. Identifying and securing these vectors is essential for building a strong cybersecurity framework.


***Linux Fundamentals:-***

Linux is an open-source operating system widely used in servers, cybersecurity, cloud computing, and development environments. Understanding basic Linux commands is essential for system administration and security tasks.

**File System Commands**

Linux follows a hierarchical file system structure starting from the root directory /.

**pwd**

Purpose: Displays the current working directory.

Example:-

pwd

Use Case:- Helps users confirm their current location in the file system.

**ls**

Purpose:- Lists files and directories in the current location.

Example:-

ls
ls -l
ls -a

Common Options:-

-l : Detailed list format

-a : Shows hidden files

**cd**

Purpose:- Changes the current directory.

Example:-

cd Documents
cd ..
cd /

Common Usage:-

cd .. → Move one directory up

cd / → Go to root directory

**File Permissions**

Linux controls access to files using permissions for:

Owner

Group

Others

Permission types:-

Read (r)

Write (w)

Execute (x)

**chmod**

Purpose:- Changes file permissions.

Example:-

chmod 755 filename
chmod +x script.sh

Explanation:-

755 means full access for owner and read/execute for others.

+x adds execute permission.

**chown**

Purpose:- Changes file ownership.

Example:-

chown user filename
chown user:group filename

Use Case: Assigns file control to a specific user or group.

**Package Management**

Linux distributions use package managers to install, update, and remove software.

**apt**

Used in Debian-based systems (like Ubuntu).

Purpose:- Install and update packages.

Example:-

sudo apt update

sudo apt install package-name

sudo apt upgrade

**dpkg**

Purpose:- Manages individual .deb packages.

Example:-

sudo dpkg -i package.deb
dpkg -l

Use Case:- Install or list locally downloaded packages.

**Networking Commands**

Networking commands help monitor and troubleshoot network connections.

**ifconfig**

Purpose:- Displays IP address and network interface details.

Example:-

ifconfig

Use Case:- Check system IP address.

**ping**

Purpose:- Tests connectivity between systems.

Example:-

ping google.com

Use Case:- Checks if a server or website is reachable.

**netstat**

Purpose:- Shows network connections, routing tables, and port status.

Example:-

netstat -tuln

Use Case:- Identify open ports and active connections.

**traceroute**

Purpose:- Displays the path packets take to reach a destination.

Example:

traceroute google.com

Use Case: Diagnose network routing issues.

**Conclusion**

These Linux fundamentals form the base for system administration and cybersecurity tasks. Mastering file system navigation, permissions, package management, and networking commands is essential for working in Linux environments.
