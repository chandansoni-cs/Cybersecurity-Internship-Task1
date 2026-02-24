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

**1. File System Commands**

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

**2.File Permissions**

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

**3.Package Management**

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

**4.Networking Commands**

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


***Networking Basics***

Networking is the process of connecting computers and devices to share data and resources. It is a fundamental concept in cybersecurity and system communication.


**1. OSI Model (Open Systems Interconnection Model)**

The OSI Model is a conceptual framework used to understand how data is transmitted over a network. It consists of 7 layers, each with a specific function.

**1. Physical Layer**

Purpose: The Physical Layer is responsible for transmitting raw bits over a physical medium.

Functions:

Data transmission through cables or wireless signals

Defines hardware elements such as cables, switches, and connectors

Examples:

Ethernet cable

USB cable

Network interface card (NIC)

**2. Data Link Layer**

Purpose: The Data Link Layer ensures reliable data transfer between two directly connected devices.

Functions:

Error detection and correction

Frame formatting

MAC address handling

Examples:

Switches

MAC addresses

Ethernet protocol

**3. Network Layer**

Purpose: The Network Layer handles logical addressing and routing of data between different networks.

Functions:

Assigns IP addresses

Determines the best path for data transmission

Examples:

IP (Internet Protocol)

Routers

**4. Transport Layer**

Purpose: The Transport Layer ensures reliable data delivery between sender and receiver.

Functions:

Data segmentation and reassembly

Error checking

Flow control

Examples:

TCP (Transmission Control Protocol)

UDP (User Datagram Protocol)

**5. Session Layer**

Purpose: The Session Layer manages communication sessions between devices.

Functions:

Establishes, maintains, and terminates sessions

Controls connections between applications

Example:

Session management in applications

**6. Presentation Layer**

Purpose: The Presentation Layer ensures data is in a readable format for the application layer.

Functions:

Data encryption and decryption

Data compression

Data format conversion

Examples:

SSL/TLS encryption

Data encoding formats

**7. Application Layer**

Purpose: The Application Layer provides network services directly to users and applications.

Functions:

Enables user interaction with network services

Provides communication interfaces

Examples:

HTTP

HTTPS

FTP

DNS

**2.TCP/IP Protocol**

Definition :- TCP/IP (Transmission Control Protocol / Internet Protocol) is the main communication protocol used for transmitting data over the internet and networks.

It defines how data is sent, received, and routed between devices.

Components of TCP/IP

TCP (Transmission Control Protocol)

Purpose: Ensures reliable and secure data transmission.

Functions:

Breaks data into packets

Ensures packets arrive correctly

Reassembles packets at destination

Example:- Used in web browsing, email, and file transfers.

**IP (Internet Protocol)**

Purpose: Provides logical addressing and routing.

Functions:

Assigns unique IP addresses

Routes packets to the correct destination

Example:- Every device connected to the internet has an IP address.

How TCP/IP Works:

Data is divided into packets by TCP

IP assigns source and destination addresses

Packets travel through the network

TCP reassembles packets at the destination

**Importance in Cybersecurity**

TCP/IP is essential because attackers often target network communication. Understanding TCP/IP helps in:

Network monitoring

Packet analysis

Detecting cyber attacks

Securing network communication


**3.DNS (Domain Name System)**

Definition:- DNS (Domain Name System) is a system that converts human-readable domain names into IP addresses.

Purpose:- Computers communicate using IP addresses, but humans use domain names. DNS translates domain names into IP addresses so computers can locate each other.

Example

When you enter:

www.google.com

DNS converts it into an IP address like:

142.250.182.14

How DNS Works

User enters a domain name in the browser

DNS server receives the request

DNS finds the corresponding IP address

The browser connects to the server using that IP address

**Importance in Cybersecurity**

Helps identify legitimate servers

Attackers may use DNS spoofing to redirect users to fake websites


**4.HTTP AND HTTPS**

**HTTP (HyperText Transfer Protocol)**

Definition:- HTTP is a protocol used for communication between web browsers and web servers.

Features:

Data is transmitted in plain text

Not secure

Vulnerable to interception

Example:

http://example.com

**HTTPS (HyperText Transfer Protocol Secure)**

Definition:- HTTPS is the secure version of HTTP. It uses SSL/TLS encryption to protect data.

Features:

Data is encrypted

Secure communication

Protects sensitive information

Example:

https://example.com

**Importance in Cybersecurity**

HTTPS protects:

Passwords

Credit card details

Personal data

**5.IP Address (Internet Protocol Address)**

Definition:- An IP Address is a unique numerical identifier assigned to each device on a network.

Purpose:- It helps devices identify and communicate with each other.

Example:- 192.168.1.1

Types of IP Address:- 1. Private IP Address

Used inside local networks.

Example:- 192.168.1.1

2. Public IP Address

Used on the internet.

Example:- 8.8.8.8

**Importance in Cybersecurity**

Helps track devices

Used in network monitoring

Helps detect unauthorized access

**6. NAT (Network Address Translation)**

Definition:- NAT (Network Address Translation) converts private IP addresses into public IP addresses to enable communication over the internet.

Purpose:- Allows multiple devices in a private network to share a single public IP address.

Example

Private IP:

192.168.1.10

Converted into Public IP:

49.36.120.15

How NAT Works

Device sends request using private IP

Router converts private IP into public IP

Request goes to the internet

Response returns to the router

Router converts public IP back to private IP

**Importance in Cybersecurity**

Hides internal network structure

Adds an extra layer of security

Helps prevent direct attacks on private devices
