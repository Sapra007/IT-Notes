# 🌐 TCP/IP Model - Complete Notes
> IT Student Notes | Topic: TCP/IP Model

---

## 📌 Table of Contents
1. [TCP/IP Model Kya Hai](#1-tcpip-model-kya-hai)
2. [TCP/IP vs OSI](#2-tcpip-vs-osi)
3. [4 Layers Detail Mein](#3-4-layers-detail-mein)
4. [TCP Kaise Kaam Karta Hai](#4-tcp-kaise-kaam-karta-hai)
5. [IP Address](#5-ip-address)
6. [DNS Kya Hota Hai](#6-dns-kya-hota-hai)
7. [Quick Revision](#7-quick-revision)

---

## 1. TCP/IP Model Kya Hai

- TCP/IP ka full form = **Transmission Control Protocol / Internet Protocol**
- Yeh **real world mein use** hone wala model hai
- OSI = Theory, TCP/IP = **Practical** ✅
- Internet isi pe kaam karta hai!

---

## 2. TCP/IP vs OSI

```
OSI Model (7 Layers)    TCP/IP Model (4 Layers)
─────────────────────   ───────────────────────
7. Application    ┐
6. Presentation   ├──→  4. Application
5. Session        ┘
4. Transport      ───→  3. Transport
3. Network        ───→  2. Internet
2. Data Link      ┐
1. Physical       ┘──→  1. Network Access
```

| | OSI | TCP/IP |
|--|-----|--------|
| Layers | 7 | 4 |
| Use | Theory | Practical ✅ |
| Purpose | Reference model | Internet standard |

---

## 3. 4 Layers Detail Mein

---

### 4️⃣ Application Layer
- User ke sabse paas
- Apps yahan kaam karti hain

| Protocol | Kaam |
|----------|------|
| **HTTP** | Web browsing |
| **HTTPS** | Secure web browsing |
| **FTP** | File transfer |
| **SMTP** | Email bhejna |
| **DNS** | Domain → IP convert |
| **SSH** | Secure remote access |

---

### 3️⃣ Transport Layer
- Data ko **segments** mein todta hai
- End to end delivery ensure karta hai

#### TCP (Transmission Control Protocol):
```
✅ Reliable
✅ Error checking karta hai
✅ Order maintain karta hai
❌ Thoda slow
Use: File download, Email, Web browsing
```

#### UDP (User Datagram Protocol):
```
✅ Bahut fast
✅ Low latency
❌ Unreliable
❌ No error checking
Use: Video call, Gaming, Live streaming
```

#### TCP vs UDP:

| | TCP | UDP |
|--|-----|-----|
| Reliability | Haan ✅ | Nahi |
| Speed | Slow | Fast ✅ |
| Error Check | Haan | Nahi |
| Order | Maintain | Nahi |
| Use | File, Email | Gaming, Video |

---

### 2️⃣ Internet Layer
- IP Addressing handle karta hai
- Routing karta hai (best path dhundta hai)

| Protocol | Kaam |
|----------|------|
| **IP** | Addressing (IPv4, IPv6) |
| **ICMP** | Error reporting (ping) |
| **ARP** | IP → MAC address convert |

---

### 1️⃣ Network Access Layer
- Physical hardware handle karta hai
- Data bits mein convert karta hai

```
Includes:
- Ethernet
- WiFi
- Cables, NIC
- MAC Address
```

---

## 4. TCP Kaise Kaam Karta Hai

### 3-Way Handshake:
```
Client            Server
  |                  |
  |--- SYN ───────→ |   (Main connect karna chahta hoon)
  |                  |
  |← SYN-ACK ─────  |   (Theek hai, aa jao)
  |                  |
  |--- ACK ───────→ |   (Shukriya, connected!)
  |                  |
  |   Data Transfer Start! ✅
```

| Term | Full Form | Matlab |
|------|-----------|--------|
| **SYN** | Synchronize | Connection request |
| **ACK** | Acknowledge | Confirmation |
| **SYN-ACK** | Both | Request accepted |

---

## 5. IP Address

```
Har device ka unique address = IP Address
Jaise ghar ka address hota hai!

IPv4 → 192.168.1.1
IPv6 → 2001:0db8:85a3::8a2e:0370:7334
```

### IPv4 vs IPv6:

| | IPv4 | IPv6 |
|--|------|------|
| Bit Length | 32 bit | 128 bit |
| Example | 192.168.1.1 | 2001:db8::1 |
| Total Addresses | ~4 billion | Almost infinite |
| Status | Common | Future ✅ |
| Format | Decimal | Hexadecimal |

### IP Address ke Parts (IPv4):
```
192  .  168  .  1  .  1
 ↑       ↑      ↑    ↑
Part1  Part2  Part3  Part4
(0-255 har part mein)
```

### IP Address Types:

| Type | Range | Use |
|------|-------|-----|
| **Private** | 192.168.x.x | Ghar/Office network |
| **Public** | Baaki sab | Internet |
| **Loopback** | 127.0.0.1 | Apna hi computer |

---

## 6. DNS Kya Hota Hai

> DNS = **"Internet ka Phone Book"**

```
Tum type karte ho: www.google.com
                        ↓
              DNS Server dhundta hai
                        ↓
          IP Address milta hai: 142.250.80.46
                        ↓
              Google open ho jaata hai! ✅
```

### DNS kaise kaam karta hai:
```
Step 1: Browser mein google.com type kiya
Step 2: Browser ne DNS server se puchha
Step 3: DNS ne IP address diya (142.250.80.46)
Step 4: Browser us IP pe gaya
Step 5: Google ka page aaya ✅
```

---

## 7. Quick Revision

### 4 Layers Summary:
```
4️⃣ Application  → HTTP, HTTPS, FTP, SMTP, DNS, SSH
3️⃣ Transport    → TCP (reliable), UDP (fast)
2️⃣ Internet     → IP, ICMP, ARP
1️⃣ Network Access → Ethernet, WiFi, Cables
```

### Important Protocols:
```
HTTP   → Web (port 80)
HTTPS  → Secure web (port 443)
FTP    → File transfer (port 21)
SMTP   → Email send (port 25)
DNS    → Domain to IP (port 53)
SSH    → Secure remote (port 22)
```

### Key Concepts:
```
TCP          = Reliable, slow, 3-way handshake
UDP          = Fast, unreliable, no handshake
IP Address   = Device ka unique address
DNS          = Domain name → IP address
3-Way Handshake = SYN → SYN-ACK → ACK
```

---

*Notes by: IT Student*
*Topic: Computer Networks - TCP/IP Model*
