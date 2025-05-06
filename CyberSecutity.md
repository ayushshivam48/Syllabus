# 📘 Module I: Introduction to Information, Computer, and Network Security

## 1. Introduction to Information, Computer, and Network Security

### 🔐 What is Information Security?

Information Security (InfoSec) is the practice of protecting **data** (both digital and physical) from **unauthorized access**, **modification**, or **destruction**.

### 🔍 What is Computer Security?

Computer Security involves protecting **computers** and their components (hardware, software, data) from **theft, damage, or disruption**.

### 🌐 What is Network Security?

Network Security focuses on safeguarding the **integrity**, **confidentiality**, and **availability** of data as it is transmitted over a network.

### 🔄 Relationship:

- Information Security is broader.
- Computer and Network Security are subsets of InfoSec.
- All aim to **protect assets** from threats.

---

## 2. Security Concepts

### 🔑 Core Concepts:

1. **Asset**: Anything valuable (e.g., data, software, hardware).
2. **Threat**: A potential cause of harm (e.g., hacker, virus).
3. **Vulnerability**: A weakness that can be exploited.
4. **Risk**: Probability of a threat exploiting a vulnerability.
5. **Control (Countermeasure)**: A safeguard to reduce risk.

---

## 3. Kinds of Security Breaches

Security breaches occur when unauthorized access or changes are made to data or systems.

### 🛠️ Types of Breaches:

1. **Data Breach**: Exposure of confidential information.
2. **System Breach**: Gaining control of a system.
3. **Physical Breach**: Unauthorized physical access.
4. **Network Breach**: Unauthorized access over a network.

---

## 4. Threats and Risks

### 🔥 Threats:

- **Malware**: Viruses, worms, trojans
- **Phishing**: Fraudulent emails to steal data
- **Denial of Service (DoS)**: Overloading systems
- **Insider Threats**: Employees misusing access

### ⚖️ Risks:

- Risk = Threat × Vulnerability × Impact
- Risk management involves identifying, assessing, and reducing risks using controls.

---

## 5. Point of Vulnerability

A **point of vulnerability** is any location in a system where security may be weak or exploitable.

### Examples:

- Weak passwords
- Outdated software
- Open ports
- Unprotected data storage

---

## 6. Attacks – Passive and Active

### 📡 Passive Attacks:

- **Goal**: Eavesdropping or monitoring
- **Do not alter data**
- Examples:
  - Traffic analysis
  - Intercepting emails

### 💣 Active Attacks:

- **Goal**: Alter or disrupt data/system
- **Direct interference**
- Examples:
  - DoS attacks
  - Man-in-the-middle
  - Spoofing
  - Malware injection

---

## 7. Security Services

Security services protect information and systems. They implement security policies and mechanisms.

### 🔐 1. Confidentiality:

- Prevent unauthorized access to information.
- Techniques: Encryption, access control.

### 🧾 2. Authentication:

- Verifies identity of users or systems.
- Techniques: Passwords, biometrics, digital certificates.

### 🛑 3. Access Control:

- Ensures only authorized users can access certain data or resources.
- Types: Discretionary (DAC), Mandatory (MAC), Role-based (RBAC).

### 🛡️ 4. Integrity:

- Ensures data is not altered in transit or storage.
- Techniques: Hashing (SHA, MD5), Digital Signatures.

### 📄 5. Non-Repudiation:

- Ensures sender cannot deny sending the message.
- Techniques: Digital signatures, timestamps, logs.

### ⚙️ 6. Availability:

- Ensures systems are accessible and functioning.
- Protected against: DoS attacks, hardware failures.

---

## 8. Model for Internetwork Security

A general model shows how security functions are embedded in communication systems.

### 🔄 General Internetwork Security Model:

Sender --> [Security Transformation] --> Communication Channel --> [Security Transformation] --> Receiver


### 🔑 Components:

- **Message**: Data to be protected
- **Security Transformations**: Encrypting, signing
- **Key**: Secret/shared key used in encryption
- **Security Policy**: Rules to enforce
- **Trusted Third Parties**: Key distribution, authentication (e.g., Certificate Authorities)

---

## 9. Internet Standards and RFCs

### 🌐 Internet Standards:

- Created by **IETF (Internet Engineering Task Force)**.
- Define protocols like TCP/IP, HTTP, DNS, SSL.

### 📃 RFC (Request for Comments):

- Documents published by IETF.
- Describe protocols, procedures, and policies.
- Each RFC is uniquely numbered.

### 🔑 Examples:

- **RFC 791**: IPv4
- **RFC 5246**: TLS v1.2
- **RFC 2616**: HTTP 1.1

---

### 🧠 Summary Points for Quick Revision:

| Concept         | Description                              |
| --------------- | ---------------------------------------- |
| Confidentiality | Data privacy (encryption)                |
| Authentication  | Identity verification                    |
| Access Control  | Restrict unauthorized access             |
| Integrity       | Data remains unaltered                   |
| Non-Repudiation | Proof of action                          |
| Availability    | System uptime and reliability            |
| Passive Attack  | Observes only                            |
| Active Attack   | Modifies/disrupts                        |
| RFC             | Official internet protocol documentation |
| Vulnerability   | Weak point in system                     |
