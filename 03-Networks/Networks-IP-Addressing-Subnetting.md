# 🌐 IP Addressing & Subnetting - Complete Notes
> IT Student Notes | Topic: IP Addressing & Subnetting

---

## 📌 Table of Contents
1. [IP Address Kya Hai](#1-ip-address-kya-hai)
2. [IPv4 Address Structure](#2-ipv4-address-structure)
3. [IP Address Classes](#3-ip-address-classes)
4. [Private vs Public IP](#4-private-vs-public-ip)
5. [Subnet Mask](#5-subnet-mask)
6. [CIDR Notation](#6-cidr-notation)
7. [Subnetting](#7-subnetting)
8. [Quick Revision](#8-quick-revision)

---

## 1. IP Address Kya Hai

- Har device ka **unique address** hota hai network mein
- Jaise ghar ka address hota hai!
- Data sahi jagah pahunche isliye IP address zaroori hai

```
Bina IP Address ke:
Data → Kahan jaaye? ❌

IP Address ke saath:
Data → 192.168.1.5 → Sahi device pe pahuncha ✅
```

---

## 2. IPv4 Address Structure

```
192  .  168  .  1  .  1
 ↑       ↑      ↑    ↑
8 bits  8 bits 8 bits 8 bits
         = 32 bits total
```

### Har Part = Octet (8 bits):
```
Range: 0 - 255 har octet mein
Example: 192.168.1.1
Minimum: 0.0.0.0
Maximum: 255.255.255.255
```

### Binary Example:
```
192        .  168       .  1         .  1
11000000   .  10101000  .  00000001  .  00000001
```

---

## 3. IP Address Classes

| Class | Range | Default Subnet | Use |
|-------|-------|----------------|-----|
| **A** | 1.0.0.0 - 126.255.255.255 | 255.0.0.0 | Bahut bade networks |
| **B** | 128.0.0.0 - 191.255.255.255 | 255.255.0.0 | Medium networks |
| **C** | 192.0.0.0 - 223.255.255.255 | 255.255.255.0 | Small networks ✅ |
| **D** | 224.0.0.0 - 239.255.255.255 | - | Multicasting |
| **E** | 240.0.0.0 - 255.255.255.255 | - | Research only |

### Class A, B, C Hosts:
```
Class A → 1 network part + 3 host parts = 16 million hosts
Class B → 2 network parts + 2 host parts = 65,534 hosts
Class C → 3 network parts + 1 host part  = 254 hosts
```

---

## 4. Private vs Public IP

### Private IP (Local Network):
| Type | Range | Use |
|------|-------|-----|
| **Class A Private** | 10.0.0.0 - 10.255.255.255 | Bade networks |
| **Class B Private** | 172.16.0.0 - 172.31.255.255 | Medium networks |
| **Class C Private** | 192.168.0.0 - 192.168.255.255 | Ghar/Office ✅ |
| **Loopback** | 127.0.0.1 | Apna hi computer |

### Public IP:
- Internet pe use hoti hai
- ISP assign karta hai
- Poori duniya mein unique hoti hai

### Private vs Public:
| | Private | Public |
|--|---------|--------|
| Use | Local network | Internet |
| Unique | Sirf local | Globally |
| Example | 192.168.1.1 | 103.21.244.0 |
| Cost | Free | ISP deta hai |

### NAT (Network Address Translation):
```
Private IP → Router (NAT) → Public IP → Internet

Ghar ke sabhi devices:
192.168.1.2 ┐
192.168.1.3 ├──→ Router ──→ 103.21.244.0 ──→ Internet
192.168.1.4 ┘
```

---

## 5. Subnet Mask

### Subnet Mask kya hota hai:
```
IP Address:   192.168.1.100
Subnet Mask:  255.255.255.0

Batata hai:
- Kaun sa part = Network
- Kaun sa part = Host (Device)
```

### Example:
```
255  .  255  .  255  .  0
─────────────────────    ─
     Network Part        Host Part
     (Fixed rehta hai)   (Change hota hai)

192.168.1.100 mein:
Network = 192.168.1
Host    = 100
```

### Subnet Mask Binary:
```
255      .  255      .  255      .  0
11111111 .  11111111 .  11111111 .  00000000
1 = Network bit
0 = Host bit
```

---

## 6. CIDR Notation

```
192.168.1.0 / 24

/24 matlab:
- 24 bits = Network ke liye
- 8 bits  = Host ke liye
- 2^8 = 256 addresses
- 254 usable (1st aur last reserved)
```

### Reserved Addresses:
```
192.168.1.0   → Network Address (use nahi hota)
192.168.1.255 → Broadcast Address (use nahi hota)
192.168.1.1 - 192.168.1.254 → Usable ✅
```

### Common CIDR Table:

| CIDR | Subnet Mask | Total Addresses | Usable Hosts |
|------|-------------|-----------------|--------------|
| /8 | 255.0.0.0 | 16,777,216 | 16,777,214 |
| /16 | 255.255.0.0 | 65,536 | 65,534 |
| /24 | 255.255.255.0 | 256 | 254 ✅ |
| /25 | 255.255.255.128 | 128 | 126 |
| /26 | 255.255.255.192 | 64 | 62 |
| /27 | 255.255.255.224 | 32 | 30 |
| /28 | 255.255.255.240 | 16 | 14 |
| /30 | 255.255.255.252 | 4 | 2 |

---

## 7. Subnetting

### Subnetting kya hota hai:
```
Ek bada network → Chhote parts mein todna = SUBNETTING

Example:
192.168.1.0/24 (254 devices)
        ↓
Subnet 1: 192.168.1.0/26   (62 devices) → HR Dept
Subnet 2: 192.168.1.64/26  (62 devices) → IT Dept
Subnet 3: 192.168.1.128/26 (62 devices) → Finance
Subnet 4: 192.168.1.192/26 (62 devices) → Admin
```

### Subnetting Kyun Karte Hain:
```
✅ Security     → Departments alag alag
✅ Performance  → Traffic kam hoti hai
✅ Management   → Easy to manage
✅ IP Wastage   → Kam hoti hai
```

### Subnetting Example Step by Step:
```
Problem: 192.168.1.0/24 ko 4 subnets mein todo

Step 1: 4 subnets chahiye = 2^2 = 4
        Isliye 2 bits borrow karo

Step 2: /24 + 2 = /26

Step 3: Har subnet mein:
        2^6 = 64 addresses
        64 - 2 = 62 usable hosts

Step 4: Subnets:
Subnet 1: 192.168.1.0   - 192.168.1.63   (/26)
Subnet 2: 192.168.1.64  - 192.168.1.127  (/26)
Subnet 3: 192.168.1.128 - 192.168.1.191  (/26)
Subnet 4: 192.168.1.192 - 192.168.1.255  (/26)
```

---

## 8. Quick Revision

```
IP Address   = Device ka unique address
IPv4         = 32 bit, 4 octets (0-255)
IPv6         = 128 bit, future use

Class A      = 1-126, bade networks
Class B      = 128-191, medium networks
Class C      = 192-223, small networks ✅

Private IP   = Local network (192.168.x.x)
Public IP    = Internet pe
Loopback     = 127.0.0.1 (apna computer)

Subnet Mask  = Network aur host part batata hai
/24          = 255.255.255.0 = 254 hosts
CIDR         = /24 jaisi short notation

Subnetting   = Bade network ko chhote mein todna
NAT          = Private IP → Public IP convert
```

### Important Numbers:
```
/24 = 254 hosts      (Most common) ✅
/25 = 126 hosts
/26 = 62 hosts
/27 = 30 hosts
/28 = 14 hosts
/30 = 2 hosts        (Point to point links)
```

---

*Notes by: IT Student*

*Topic: Computer Networks - IP Addressing & Subnetting*
