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



# 📘 Module II: Cyber Security

---

## 1. Sources of Security Threats

### 🔍 Categories:

- **External Threats**: Hackers, cybercriminals, foreign governments.
- **Internal Threats**: Employees, contractors, trusted users.
- **Natural Threats**: Earthquakes, floods, power outages.
- **Human Errors**: Unintentional mistakes (e.g., misconfiguration).

---

## 2. Motives Behind Attacks

### 💡 Common Motives:

- Financial Gain (e.g., stealing credit card info)
- Espionage (government or corporate)
- Political Agenda (hacktivism)
- Revenge (disgruntled employees)
- Fun or Challenge (script kiddies, black hat hackers)
- Terrorism or Sabotage

---

## 3. Target Assets

### 🎯 Examples:

- Personal data (SSN, passwords)
- Financial information (bank details)
- Intellectual property (patents, source code)
- Business data (client info, strategies)
- Critical Infrastructure (power grids, airports)

---

## 4. Consequences of Threats

### ⚠️ Impacts:

- Data loss or leakage
- Financial loss
- Legal consequences
- Reputational damage
- Service downtime
- Physical damage (in cyber-physical systems)

---

## 5. Types of Cyber Threats

### ✉️ **Email Threats**:

- **Phishing**: Fake emails to steal information.
- **Spoofing**: Sending emails that look like they're from trusted sources.
- **Malware attachments**: Carry viruses or trojans.

### 🌐 **Web Threats**:

- **Drive-by Downloads**: Downloading malware from compromised websites.
- **Clickjacking**: Misleading users to click hidden links.
- **Fake websites**: Look like real ones to steal login credentials.

### 💻 **Hacking**:

- Unauthorized access to systems.
- Types: White-hat (ethical), black-hat (malicious), grey-hat (in between).

### 🕵️‍♂️ **Intruders**:

- Individuals who gain unauthorized access.
  - **Masquerader**: Outside attacker using stolen credentials.
  - **Misfeasor**: Insider misusing privileges.
  - **Clandestine user**: Hides their presence.

### 🏢 **Insider Threats**:

- Employees or authorized users who misuse access.
- Often harder to detect due to valid credentials.

---

## 6. Cyber Crimes

### 👥 **Cyber Squatting**:

- Registering domain names similar to real trademarks to sell later at a profit.

### 🕵️‍♀️ **Cyber Stalking**:

- Repeated harassment using electronic communications.
- Involves monitoring, threats, or false accusations.

### 🎭 **Crime of Deception**:

- Using false identities or trickery to commit fraud (e.g., fake profiles, scam emails).

### 📄 **Content-Oriented Online Crime**:

- Distribution of illegal or harmful content:
  - Child pornography
  - Hate speech
  - Pirated software or media

---

## 7. Malicious Software (Malware)

### 🧬 Types:

- **Virus**: Attaches to files and spreads when executed.
- **Worm**: Self-replicating, spreads without user action.
- **Trojan Horse**: Appears useful but has malicious code.
- **Spyware**: Monitors user activity.
- **Adware**: Unwanted ads.
- **Ransomware**: Encrypts files and demands ransom.

### 🛠️ Detection:

- Antivirus software
- Intrusion Detection Systems (IDS)
- Behavioral analysis tools

---

## 8. Cyber Terrorism

### 🔥 Definition:

- Use of the internet to conduct violent acts that threaten or cause fear.
- Targets: power grids, air traffic, financial systems.

---

## 9. Information Warfare and Surveillance

### 🛰️ Information Warfare:

- Using information and communication technology to gain competitive or strategic advantage in conflicts.

### 👁️ Surveillance:

- Monitoring digital activity (can be legal or illegal).
- Used by governments, ISPs, or malicious actors.

---

## 10. Virtual Crime & Online Frauds

### 🌐 Virtual Crime:

- Crimes occurring purely in the digital world (e.g., hacking virtual goods, online gaming scams).

### 💳 Online Frauds:

- Credit card fraud, lottery scams, fake shopping sites, job frauds.

---

## 11. Identity Theft & Intellectual Property Theft

### 🧑‍💼 Identity Theft:

- Stealing personal information to impersonate someone else.
- Used for fraud, fake accounts, etc.

### 🧠 Intellectual Property Theft:

- Stealing copyrighted or patented materials like software, designs, trademarks.

---

## 12. Network Threats

| Threat Type | Description                                                    |
| ----------- | -------------------------------------------------------------- |
| **Worms**   | Self-replicating programs that spread through networks.        |
| **Virus**   | Inserts malicious code into host files.                        |
| **Spam**    | Unsolicited bulk messages, often carrying malware or phishing. |
| **Adware**  | Displays intrusive ads, may track user behavior.               |
| **Spyware** | Secretly monitors user activity and sends data to attackers.   |

---

## 13. Other Attacks & Concepts

### 🐴 Trojans:

- Malware disguised as legitimate software.
- Used to create backdoors for hackers.

### 🔗 Covert Channels:

- Unintended communication paths used to leak data.

### 🔓 Backdoors:

- Secret access methods into a system, bypassing normal authentication.

### 🤖 Bots:

- Infected devices controlled by attackers (botnets).
- Used for spam, DDoS attacks, crypto mining.

### 🎭 IP Spoofing:

- Faking the source IP address in packets to hide identity or impersonate.

### 🌐 ARP Spoofing:

- Sending fake ARP messages to link attacker's MAC to another IP address.
- Enables Man-in-the-Middle attacks.

### 🧠 Session Hijacking:

- Taking over a user session after authentication by stealing session tokens.

### 💥 Sabotage:

- Intentional damage or destruction to systems or data.

### 🎣 Phishing:

- Tricking users into revealing sensitive data via fake websites/emails.

### 🧟 Zombie / Zombie Drone:

- A compromised computer remotely controlled by an attacker.
- Often part of a botnet.

---

## 🧠 Quick Revision Table

| Attack Type | Key Feature                      |
| ----------- | -------------------------------- |
| Virus       | Needs a host file                |
| Worm        | Self-replicating                 |
| Trojan      | Disguised as legitimate software |
| Spyware     | Monitors activity                |
| Adware      | Shows ads                        |
| Phishing    | Social engineering via email     |
| Spoofing    | Faking identity/IP               |
| Hijacking   | Taking over sessions             |
| Backdoor    | Secret access                    |
| Botnet      | Group of zombie machines         |

