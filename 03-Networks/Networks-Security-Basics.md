# 🔒 Network Security Basics - Complete Notes
> IT Student Notes | Topic: Network Security

---

## 📌 Table of Contents
1. [Network Security Kya Hai](#1-network-security-kya-hai)
2. [Types of Attacks](#2-types-of-attacks)
3. [Defense Tools](#3-defense-tools)
4. [Encryption](#4-encryption)
5. [Quick Revision](#5-quick-revision)

---

## 1. Network Security Kya Hai

- Network ko **unauthorized access** se bachana
- Data ko **safe** rakhna
- Attacks se **protect** karna

```
Bina Security:
Internet → Network → Koi bhi access kar sakta hai ❌

Security ke saath:
Internet → Firewall → Network → Safe ✅
```

---

## 2. Types of Attacks

---

### 1. 🦠 Malware
- Malicious software hota hai
- Computer ko **harm** karta hai

| Type | Kaam |
|------|------|
| **Virus** | Files mein spread hota hai |
| **Worm** | Network mein khud spread karta hai |
| **Trojan** | Useful lagta hai but harmful hai |
| **Ransomware** | Data lock karke paise maangta hai |
| **Spyware** | Secretly data churaata hai |
| **Adware** | Unwanted ads dikhata hai |

---

### 2. 🎣 Phishing
- Fake emails/websites se **data churana**
- User ko fool karta hai

```
Real:  https://sbi.co.in       ✅
Fake:  https://sbi-login.xyz   ❌ Phishing!
```

#### Types:
| Type | Kaam |
|------|------|
| **Email Phishing** | Fake email bhejta hai |
| **Spear Phishing** | Specific person ko target |
| **Smishing** | SMS se phishing |
| **Vishing** | Voice call se phishing |

---

### 3. 🔁 DoS / DDoS Attack
- **DoS** = Denial of Service
- Server ko **requests se overwhelm** karna
- Server crash ho jaata hai!

```
Normal:
User → Request → Server ✅

DoS:
Attacker → Millions of requests → Server 💥

DDoS (Distributed):
PC1 ┐
PC2 ├── Millions of requests → Server 💥
PC3 ┘
(Multiple computers se attack)
```

| | DoS | DDoS |
|--|-----|------|
| Source | Ek computer | Multiple computers |
| Power | Kam | Zyada |
| Detect | Easy | Hard |

---

### 4. 👤 Man in the Middle (MITM)
- Attacker **beech mein** baith jaata hai
- Data **intercept** karta hai

```
Normal:
User ←──────────────→ Server

MITM:
User ←→ Attacker ←→ Server
         👀 Sab dekh raha hai!
```

#### MITM se kaise bachein:
```
✅ HTTPS use karo
✅ VPN use karo
✅ Public WiFi pe sensitive kaam mat karo
```

---

### 5. 💉 SQL Injection
- Database mein **malicious code** inject karna
- Data chura sakte hain

```
Normal query:
SELECT * FROM users WHERE id=1

Injected query:
SELECT * FROM users WHERE id=1 OR 1=1
                          ↑
                  Sab users mil gaye! ❌
```

---

### 6. 🔑 Brute Force Attack
- **Har possible password** try karna
- Time lagta hai but kaam karta hai

```
Try: password1 ❌
Try: password2 ❌
Try: abc123    ❌
Try: admin123  ✅ Mil gaya!
```

#### Brute Force se kaise bachein:
```
✅ Strong password use karo
✅ 2FA enable karo
✅ Account lockout enable karo
```

---

## 3. Defense Tools

---

### 1. 🔥 Firewall
- Network ka **"Security Guard"**
- Allowed aur blocked traffic decide karta hai

```
Internet → [FIREWALL] → Network
              ↓
    Rules check karta hai:
    ✅ Port 80  → Allow (HTTP)
    ✅ Port 443 → Allow (HTTPS)
    ❌ Port 23  → Block (Telnet)
    ❌ Unknown IPs → Block
```

#### Firewall ke Types:
| Type | Feature |
|------|---------|
| **Packet Filter** | Basic, IP/Port check |
| **Stateful** | Connection track karta hai |
| **Application** | Deep inspection ✅ |
| **Next-Gen (NGFW)** | AI based, advanced ✅ |

---

### 2. 🔒 VPN (Virtual Private Network)
- **Encrypted tunnel** banata hai
- Public network pe private connection

```
Tumhara PC → [VPN Tunnel 🔒] → Internet
              (Encrypted!)

Benefits:
✅ Data encrypted
✅ IP address hide
✅ Public WiFi safe
✅ Remote work possible
```

---

### 3. 🕵️ IDS / IPS
- **IDS** = Intrusion Detection System
- **IPS** = Intrusion Prevention System

```
IDS → Sirf alert karta hai ⚠️
IPS → Attack block karta hai 🛑
```

| | IDS | IPS |
|--|-----|-----|
| Kaam | Detect karna | Prevent karna |
| Action | Alert bhejta hai | Block karta hai |
| Position | Network monitor | Inline (beech mein) |

---

### 4. 🛡️ Antivirus / Antimalware
- Malware **detect aur remove** karta hai
- Real-time protection deta hai

```
File download kiya
      ↓
Antivirus scan kiya
      ↓
Safe hai? ✅ → Allow
Virus hai? ❌ → Block + Remove
```

---

### 5. 🔐 DMZ (Demilitarized Zone)
- Public servers ko **alag zone** mein rakhna
- Internal network safe rehta hai

```
Internet → [Firewall 1] → DMZ (Web servers)
                        → [Firewall 2] → Internal Network
```

---

## 4. Encryption

- Data ko **scramble** karta hai
- Bina key ke padhna impossible

```
Plain text:  "Hello World"
Encrypted:   "X7#mK9@Qz2"
Decrypted:   "Hello World" ✅
```

### Encryption ke Types:

#### Symmetric Encryption:
```
Ek hi key encrypt aur decrypt ke liye

Sender: Hello → [Key 🔑] → X7#mK9
Receiver: X7#mK9 → [Key 🔑] → Hello ✅

Fast hai but key share karna risky
Example: AES
```

#### Asymmetric Encryption:
```
2 keys: Public Key + Private Key

Sender: Hello → [Public Key 🔓] → X7#mK9
Receiver: X7#mK9 → [Private Key 🔒] → Hello ✅

Slow hai but secure
Example: RSA, SSL/TLS
```

| | Symmetric | Asymmetric |
|--|-----------|------------|
| Keys | 1 | 2 (Public + Private) |
| Speed | Fast ✅ | Slow |
| Security | Medium | High ✅ |
| Example | AES | RSA, SSL |

### SSL/TLS:
```
HTTPS = HTTP + SSL/TLS
Browser aur server ke beech encrypted connection

Kaise pata chalega?
🔒 Lock icon browser mein ✅
https:// se shuru ✅
```

---

## 5. Quick Revision

### Attacks Summary:
```
🦠 Malware      → Virus, Worm, Trojan, Ransomware
🎣 Phishing     → Fake email/website se data chori
🔁 DoS/DDoS     → Server ko overwhelm karna
👤 MITM         → Beech mein baith ke data dekhna
💉 SQL Injection → Database mein malicious code
🔑 Brute Force  → Har password try karna
```

### Defense Summary:
```
🔥 Firewall     → Traffic filter karta hai
🔒 VPN          → Encrypted tunnel
🕵️ IDS/IPS      → Attack detect/prevent
🛡️ Antivirus    → Malware remove karta hai
🔐 Encryption   → Data scramble karta hai
```

### Important Terms:
```
Malware    = Malicious software
Phishing   = Fake identity se data chori
DoS        = Server crash karna
MITM       = Man in the Middle
Firewall   = Network ka security guard
VPN        = Virtual Private Network
IDS        = Intrusion Detection System
IPS        = Intrusion Prevention System
AES        = Symmetric encryption
RSA        = Asymmetric encryption
SSL/TLS    = HTTPS encryption protocol
```

---

*Notes by: IT Student*
*Topic: Computer Networks - Network Security Basics*
