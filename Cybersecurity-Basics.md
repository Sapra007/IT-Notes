# 🔐 Cybersecurity - Basics
> IT Student Notes | Topic: Cybersecurity Fundamentals

---

## 📌 Table of Contents
1. [Cybersecurity Kya Hai](#1-cybersecurity-kya-hai)
2. [CIA Triad](#2-cia-triad)
3. [Types of Threats](#3-types-of-threats)
4. [Common Attacks](#4-common-attacks)
5. [Important Terms](#5-important-terms)
6. [Encryption Basics](#6-encryption-basics)
7. [Network Security](#7-network-security)
8. [Quick Revision](#8-quick-revision)

---

## 1. Cybersecurity Kya Hai

- **Digital systems, networks aur data** ko attacks se bachana
- Unauthorized access, damage ya theft se protection
- Example: Bank ka online system secure karna, personal data protect karna

### Physical Security vs Cybersecurity:

| | Physical Security | Cybersecurity |
|--|------------------|---------------|
| Protect karta hai | Buildings, hardware | Data, networks, software |
| Threat | Chor, aag | Hacker, virus, malware |
| Tools | Lock, CCTV | Firewall, antivirus, encryption |
| Visible | Haan ✅ | Mostly nahi ❌ |
| Example | Gate lock | Password, firewall |

---

## 2. CIA Triad

> Cybersecurity ki **sabse important foundation** — Teen pillars:

```
        🔐 CIA TRIAD
        
   C → Confidentiality  (Privacy)
   I → Integrity        (Accuracy)
   A → Availability     (Access)
```

### C — Confidentiality (Gupt rehna):
- Data sirf **authorized logon** ko dikhna chahiye
- Example: Tera bank password sirf tujhe pata hona chahiye
- Tools: Encryption, Password, Access Control

### I — Integrity (Sahi rehna):
- Data **accurate aur unmodified** rehna chahiye
- Example: Tere marks koi badal na sake
- Tools: Hashing, Digital Signature, Checksums

### A — Availability (Available rehna):
- System aur data **hamesha accessible** rehna chahiye
- Example: ATM hamesha kaam kare, website down na ho
- Tools: Backup, Load Balancing, Disaster Recovery

---

## 3. Types of Threats

### Threats ke Types:

| Type | Matlab | Example |
|------|--------|---------|
| **Malware** | Harmful software | Virus, Ransomware |
| **Phishing** | Fake link/email se data chori | Fake bank email |
| **DoS/DDoS** | Server ko overload karna | Website crash |
| **Man-in-Middle** | Beech mein baith ke data sunna | WiFi snooping |
| **SQL Injection** | Database pe attack | Login bypass |
| **Social Engineering** | Insaan ko fool karna | Fake call se password lena |

### Threat Actors (Kaun karta hai):

```
👤 Script Kiddie   → Beginner hacker, ready-made tools use karta hai
🧑‍💻 Hacker          → Skilled attacker
🏛️ Nation State     → Government-backed cyber attack
😈 Insider Threat  → Company ka apna hi employee
🤖 Botnet          → Infected computers ka group
```

---

## 4. Common Attacks

### Malware Types:

```
Virus       → File se attach hota hai, spread karta hai
Worm        → Khud hi spread karta hai (no file needed)
Trojan      → Useful software jaisa dikhta hai, par harmful
Ransomware  → Files encrypt karta hai, paise maangta hai
Spyware     → Secretly activity monitor karta hai
Adware      → Unwanted ads dikhata hai
Rootkit     → System mein deep chhup jaata hai
```

### Phishing:

```
Normal Phishing  → Bulk fake emails bhejna
Spear Phishing   → Specific person ko target karna
Whaling          → CEO/Boss ko target karna
Vishing          → Voice call se fool karna (Voice + Phishing)
Smishing         → SMS se fool karna (SMS + Phishing)
```

### SQL Injection Example:

```sql
-- Normal Login Query:
SELECT * FROM users WHERE username='rahul' AND password='1234';

-- Attacker ne type kiya:
username: admin'--
-- Query ban gayi:
SELECT * FROM users WHERE username='admin'--' AND password='...';
-- Password check hi nahi hua! 😱
```

### DoS vs DDoS:

| | DoS | DDoS |
|--|-----|------|
| Full Form | Denial of Service | Distributed DoS |
| Attacker | 1 system | 1000s of systems |
| Danger | Kam | Zyada ✅ |
| Example | Ek computer se spam | Botnet se attack |

---

## 5. Important Terms

| Term | Matlab | Example |
|------|--------|---------|
| **Vulnerability** | System ki weakness | Unpatched software |
| **Exploit** | Vulnerability use karna | Attack code |
| **Threat** | Potential danger | Hacker |
| **Risk** | Threat + Vulnerability | Hacker + Weak password |
| **Firewall** | Network traffic filter | Port blocker |
| **VPN** | Encrypted tunnel | Safe browsing |
| **Patch** | Bug fix update | Windows Update |
| **Zero-Day** | Unknown vulnerability | Newly found bug |
| **Penetration Test** | Legal hacking (testing) | Security audit |
| **2FA** | 2 step verification | OTP + Password |

### Hacker Types:

```
⚪ White Hat  → Ethical hacker (legal, company hire karta hai)
⚫ Black Hat  → Malicious hacker (illegal)
🔘 Grey Hat   → Beech mein (sometimes legal, sometimes not)
```

---

## 6. Encryption Basics

- Data ko **unreadable format** mein convert karna
- Sirf authorized person hi decrypt kar sake

```
Plain Text  →  [Encryption]  →  Cipher Text
"Hello"     →  [AES-256]     →  "X7#kP!9mQ"

Cipher Text →  [Decryption]  →  Plain Text
"X7#kP!9mQ" →  [Key]         →  "Hello"
```

### Symmetric vs Asymmetric:

| | Symmetric | Asymmetric |
|--|-----------|------------|
| Keys | 1 same key (encrypt + decrypt) | 2 keys (Public + Private) |
| Speed | Fast ✅ | Slow |
| Use | File encryption | HTTPS, Email |
| Example | AES, DES | RSA, ECC |

### HTTPS kaise kaam karta hai:

```
Browser          Server
   |                |
   |--- Hello ----→ |
   |←-- Certificate |  (Server ka Public Key)
   |--- Session Key →|  (Public key se encrypt)
   |←-→ Encrypted ---→|  (Ab safe communication)
```

### Hashing:

```
Password  →  [Hash Function]  →  Hash Value
"pass123" →  [SHA-256]        →  "ef92b778baf..."

Properties:
✅ One-way  (reverse nahi ho sakta)
✅ Same input = Same output hamesha
✅ Thoda sa change = Poora hash badal jaata hai
```

---

## 7. Network Security

### Firewall:

```
Internet → [FIREWALL] → Internal Network

Firewall decide karta hai:
✅ Allow → Safe traffic
❌ Block → Suspicious traffic

Types:
- Packet Filtering  → Basic rules (IP/Port)
- Stateful          → Connection track karta hai
- Application Layer → Deep packet inspection
```

### Common Ports to Know:

| Port | Protocol | Use |
|------|----------|-----|
| **80** | HTTP | Normal web |
| **443** | HTTPS | Secure web |
| **22** | SSH | Remote login |
| **21** | FTP | File transfer |
| **25** | SMTP | Email send |
| **3306** | MySQL | Database |
| **3389** | RDP | Remote Desktop |

### IDS vs IPS:

| | IDS | IPS |
|--|-----|-----|
| Full Form | Intrusion Detection System | Intrusion Prevention System |
| Kaam | Attack detect karta hai | Attack block karta hai |
| Action | Alert deta hai | Automatically block karta hai |
| Type | Passive | Active |

### VPN Kaise Kaam Karta Hai:

```
Tu  →  [VPN Server]  →  Internet
         ↑
    Encrypted Tunnel
    Real IP chhup jaata hai
    Safe on public WiFi ✅
```

---

## 8. Quick Revision

```
Cybersecurity = Digital systems ko attacks se bachana
CIA Triad     = Confidentiality, Integrity, Availability
Malware       = Harmful software (Virus, Worm, Trojan...)
Phishing      = Fake email/link se data chori
Ransomware    = Files lock karke paise maangna
Firewall      = Network traffic filter
Encryption    = Data ko unreadable banao
Hashing       = One-way data convert (password store)
VPN           = Encrypted internet tunnel
2FA           = 2 step login (extra security)
Vulnerability = System ki weakness
Exploit       = Vulnerability use karne ka tarika
Patch         = Bug fix (update karo!)
White Hat     = Ethical hacker ✅
Black Hat     = Malicious hacker ❌
```

### Security Best Practices:

```
✅ Strong password use karo (12+ chars, symbols)
✅ 2FA hamesha enable karo
✅ Software update karte raho (patches!)
✅ Unknown links pe click mat karo
✅ Public WiFi pe VPN use karo
✅ Regular backups rakho
❌ Same password repeat mat karo
❌ Suspicious emails ke attachments mat kholo
```

---

*Notes by: IT Student*
*Topic: Cybersecurity - Basics*
*Phase 6 of IT Learning Path 🔐*
