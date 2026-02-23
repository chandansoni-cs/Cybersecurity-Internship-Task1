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

