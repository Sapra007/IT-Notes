# 🌐 Network Protocols - Complete Notes
> IT Student Notes | Topic: Network Protocols

---

## 📌 Table of Contents
1. [Protocol Kya Hota Hai](#1-protocol-kya-hota-hai)
2. [HTTP & HTTPS](#2-http--https)
3. [FTP](#3-ftp)
4. [Email Protocols](#4-email-protocols)
5. [DNS](#5-dns)
6. [SSH](#6-ssh)
7. [DHCP](#7-dhcp)
8. [Ports Summary](#8-ports-summary)
9. [Quick Revision](#9-quick-revision)

---

## 1. Protocol Kya Hota Hai

- Protocol = **Rules ka set**
- Computers ke beech **communication ke rules**
- Jaise insaan baat karte waqt language follow karte hain!

### Protocols ka Overview:
```
Application Layer → HTTP, HTTPS, FTP, SMTP, DNS, SSH
Transport Layer   → TCP, UDP
Internet Layer    → IP, ICMP, ARP
```

---

## 2. HTTP & HTTPS

### HTTP (HyperText Transfer Protocol):
- Web pages **browse** karne ke liye
- Port **80**
- Data encrypted nahi hota ❌

### HTTPS (HTTP Secure):
- HTTP + **SSL/TLS encryption**
- Port **443**
- Data **encrypted** hota hai ✅
- Bank, shopping sites pe use hota hai

```
HTTP  → http://website.com  (Unsafe ❌)
HTTPS → https://website.com (Safe ✅)
```

### HTTP Request/Response:
```
Browser → Request bheja → Server
             GET /index.html
                  ↓
Server → Response bheja → Browser
             200 OK + Page data
```

### HTTP Methods:
| Method | Kaam |
|--------|------|
| **GET** | Data maangna |
| **POST** | Data bhejna |
| **PUT** | Data update karna |
| **DELETE** | Data delete karna |

### HTTP Status Codes:
| Code | Matlab |
|------|--------|
| **200** | OK - Success ✅ |
| **301** | Permanently Redirected |
| **400** | Bad Request |
| **401** | Unauthorized |
| **403** | Forbidden |
| **404** | Page Not Found ❌ |
| **500** | Server Error |

### HTTP vs HTTPS:
| | HTTP | HTTPS |
|--|------|-------|
| Security | No encryption ❌ | Encrypted ✅ |
| Port | 80 | 443 |
| Speed | Thoda fast | Thoda slow |
| Use | Old | Modern ✅ |
| Certificate | Nahi | SSL/TLS ✅ |

---

## 3. FTP

### FTP (File Transfer Protocol):
- Files **transfer** karne ke liye
- Port **21**
- Server se files upload/download karna

```
Client ──→ FTP Server
      Upload/Download files
```

### FTP vs SFTP vs FTPS:
| | FTP | SFTP | FTPS |
|--|-----|------|------|
| Security | No encryption ❌ | Encrypted ✅ | Encrypted ✅ |
| Port | 21 | 22 | 990 |
| Protocol | FTP | SSH based | FTP + SSL |
| Use | Old | Modern ✅ | Modern ✅ |

---

## 4. Email Protocols

### SMTP (Simple Mail Transfer Protocol):
- Email **bhejna** (Send)
- Port **25** ya **587**

### POP3 (Post Office Protocol v3):
- Email **download** karna
- Port **110**
- Server se delete ho jaata hai ❌
- Ek hi device pe access

### IMAP (Internet Message Access Protocol):
- Email **server pe** rehta hai
- Port **143**
- Multiple devices pe access ✅
- Server pe sync rehta hai

### Email Flow:
```
Sender → [SMTP] → Mail Server → [IMAP/POP3] → Receiver
```

### POP3 vs IMAP:
| | POP3 | IMAP |
|--|------|------|
| Storage | Local device | Server ✅ |
| Multiple devices | Nahi ❌ | Haan ✅ |
| Internet needed | Download ke baad nahi | Haan |
| Port | 110 | 143 |
| Use | Old | Modern ✅ |

---

## 5. DNS

### DNS (Domain Name System):
- Domain name → IP address convert karta hai
- Port **53**
- Internet ka **"Phone Book"**

```
google.com  → 142.250.80.46
youtube.com → 142.250.80.100
```

### DNS Resolution Step by Step:
```
Step 1: Browser mein google.com type kiya
              ↓
Step 2: Local DNS Cache check kiya
              ↓
Step 3: DNS Resolver se puchha
              ↓
Step 4: Root Server se puchha
              ↓
Step 5: TLD Server (.com) se puchha
              ↓
Step 6: Authoritative Server se IP mila
              ↓
Step 7: 142.250.80.46 → Google open! ✅
```

### DNS Record Types:
| Record | Kaam |
|--------|------|
| **A** | Domain → IPv4 address |
| **AAAA** | Domain → IPv6 address |
| **CNAME** | Domain → Domain (alias) |
| **MX** | Email server ka address |
| **NS** | Name server |

---

## 6. SSH

### SSH (Secure Shell):
- **Remote computer** access karna
- Port **22**
- Encrypted connection ✅
- Command line se remote access

```
Tum Ahmedabad mein ho →
SSH se Mumbai ka server access kar sakte ho!

Command:
ssh username@192.168.1.100
```

### SSH vs Telnet:
| | SSH | Telnet |
|--|-----|--------|
| Security | Encrypted ✅ | No encryption ❌ |
| Port | 22 | 23 |
| Use | Modern ✅ | Old, avoid |

---

## 7. DHCP

### DHCP (Dynamic Host Configuration Protocol):
- Automatically **IP address assign** karta hai
- Port **67** (Server), **68** (Client)
- Bina manually IP set kiye kaam karta hai

### DHCP Process:
```
Step 1: DISCOVER  → New device: "Koi DHCP server hai?"
Step 2: OFFER     → Server: "Haan! Yeh lo IP: 192.168.1.10"
Step 3: REQUEST   → Device: "Theek hai, mujhe yeh chahiye"
Step 4: ACK       → Server: "Done! IP tumhari hai!" ✅
```

### DHCP vs Static IP:
| | DHCP | Static IP |
|--|------|-----------|
| Setup | Automatic ✅ | Manual |
| Change | Har baar change ho sakti hai | Fixed rehti hai |
| Use | Normal devices | Servers, Printers |

---

## 8. Ports Summary

### Important Ports:
| Protocol | Port | Use |
|----------|------|-----|
| **FTP** | 21 | File transfer |
| **SSH** | 22 | Secure remote access |
| **Telnet** | 23 | Old remote access |
| **SMTP** | 25 | Email send |
| **DNS** | 53 | Domain to IP |
| **HTTP** | 80 | Web browsing |
| **POP3** | 110 | Email download |
| **IMAP** | 143 | Email server sync |
| **HTTPS** | 443 | Secure web |
| **DHCP** | 67/68 | IP assign |

### Port Ranges:
```
0    - 1023  → Well Known Ports (System ports)
1024 - 49151 → Registered Ports
49152- 65535 → Dynamic/Private Ports
```

---

## 9. Quick Revision

```
HTTP    → Web browsing, port 80, no encryption
HTTPS   → Secure web, port 443, SSL/TLS ✅
FTP     → File transfer, port 21
SFTP    → Secure file transfer, port 22 ✅
SMTP    → Email bhejna, port 25/587
POP3    → Email download, port 110
IMAP    → Email server sync, port 143 ✅
DNS     → Domain → IP, port 53
SSH     → Remote access, port 22, encrypted ✅
DHCP    → Auto IP assign, port 67/68
```

### Status Codes Trick:
```
2xx → Success ✅
3xx → Redirect
4xx → Client Error (tumhari galti)
5xx → Server Error (server ki galti)
```

---

*Notes by: IT Student*
*Topic: Computer Networks - Protocols*
