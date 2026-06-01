# 📚 OSI Model - Complete Notes
> IT Student Notes | Topic: OSI Model

---

## 📌 Table of Contents
1. [OSI Model Kya Hai](#1-osi-model-kya-hai)
2. [7 Layers Overview](#2-7-layers-overview)
3. [Har Layer Detail Mein](#3-har-layer-detail-mein)
4. [Data Units](#4-data-units)
5. [Data Kaise Travel Karta Hai](#5-data-kaise-travel-karta-hai)
6. [Quick Revision](#6-quick-revision)

---

## 1. OSI Model Kya Hai

- OSI ka full form = **Open Systems Interconnection**
- Yeh ek **standard framework** hai
- Batata hai ki network mein **data kaise travel** karta hai
- **7 layers** hoti hain!

---

## 2. 7 Layers Overview

```
7. Application Layer   ← User ke sabse paas
6. Presentation Layer
5. Session Layer
4. Transport Layer
3. Network Layer
2. Data Link Layer
1. Physical Layer      ← Hardware ke sabse paas
```

### Yaad Karne Ka Trick:
> **"All People Seem To Need Data Processing"**
> A - P - S - T - N - D - P (7 se 1 tak)

---

## 3. Har Layer Detail Mein

---

### 7️⃣ Application Layer
- User **directly interact** karta hai
- Apps yahan kaam karti hain

| Feature | Detail |
|---------|--------|
| Protocols | HTTP, HTTPS, FTP, SMTP, DNS |
| Example | Chrome, Email, WhatsApp |
| Data Unit | Data |

---

### 6️⃣ Presentation Layer
- Data ko **translate, encrypt, compress** karta hai
- Format change karta hai

| Kaam | Example |
|------|---------|
| Encryption | Data secure karna (SSL) |
| Compression | Data chhota karna |
| Translation | Format change karna |
| Formats | JPEG, MP3, MP4 |

---

### 5️⃣ Session Layer
- **Connection establish** karta hai
- Session start aur band karta hai

```
Login kiya   → Session start
Logout kiya  → Session end
Video call   → Session maintain karta hai
```

---

### 4️⃣ Transport Layer
- Data ko **segments** mein todta hai
- **Reliable delivery** ensure karta hai
- Error checking karta hai

| Protocol | Feature | Use |
|----------|---------|-----|
| **TCP** | Reliable, slow | File download, Email |
| **UDP** | Fast, unreliable | Video call, Gaming |

---

### 3️⃣ Network Layer
- **IP Address** handle karta hai
- **Routing** karta hai (Best path dhundta hai)
- Data ko **packets** mein todta hai

| Feature | Detail |
|---------|--------|
| Protocol | IP (Internet Protocol) |
| Device | Router |
| Example | 192.168.1.1 |
| Data Unit | Packets |

---

### 2️⃣ Data Link Layer
- **MAC Address** handle karta hai
- Data ko **frames** mein todta hai
- Same network mein delivery karta hai

| Feature | Detail |
|---------|--------|
| Protocol | Ethernet, WiFi |
| Device | Switch |
| Example | 00:1A:2B:3C:4D:5E |
| Data Unit | Frames |

---

### 1️⃣ Physical Layer
- **Actual hardware** hai
- Bits (0 aur 1) ko signals mein convert karta hai

| Feature | Detail |
|---------|--------|
| Devices | Cables, Hub, NIC |
| Signals | Electrical, Light, Radio waves |
| Data Unit | Bits (0s and 1s) |

---

## 4. Data Units

| Layer | Naam | Data Unit |
|-------|------|-----------|
| 7 - Application | Application | Data |
| 6 - Presentation | Presentation | Data |
| 5 - Session | Session | Data |
| 4 - Transport | Transport | Segments |
| 3 - Network | Network | Packets |
| 2 - Data Link | Data Link | Frames |
| 1 - Physical | Physical | Bits |

---

## 5. Data Kaise Travel Karta Hai

### Sender Side (Top to Bottom - Encapsulation):
```
7. Application   → Data banaya
        ↓
6. Presentation  → Encrypt kiya
        ↓
5. Session       → Connection banaya
        ↓
4. Transport     → Segments mein toda
        ↓
3. Network       → Packets mein toda + IP lagaya
        ↓
2. Data Link     → Frames mein toda + MAC lagaya
        ↓
1. Physical      → Bits mein convert → Cable se bheja 🚀
```

### Receiver Side (Bottom to Top - Decapsulation):
```
1. Physical      → Bits receive kiye
        ↑
2. Data Link     → Frames assemble kiye
        ↑
3. Network       → Packets assemble kiye
        ↑
4. Transport     → Segments assemble kiye
        ↑
5. Session       → Connection verify kiya
        ↑
6. Presentation  → Decrypt kiya
        ↑
7. Application   → User ko data mila! ✅
```

---

## 6. Quick Revision

### Layers Summary:
```
7️⃣ Application  → User interact karta hai (HTTP, FTP)
6️⃣ Presentation → Encrypt, Compress, Translate (SSL)
5️⃣ Session      → Connection manage karta hai
4️⃣ Transport    → Segments, TCP/UDP
3️⃣ Network      → Packets, IP Address, Router
2️⃣ Data Link    → Frames, MAC Address, Switch
1️⃣ Physical     → Bits, Cables, NIC
```

### Devices per Layer:
```
Layer 7, 6, 5 → Computer/Server
Layer 4       → Firewall
Layer 3       → Router
Layer 2       → Switch
Layer 1       → Cable, Hub, NIC
```

### Protocols Summary:
```
HTTP/HTTPS → Web browsing (Layer 7)
FTP        → File transfer (Layer 7)
SMTP       → Email (Layer 7)
SSL/TLS    → Encryption (Layer 6)
TCP        → Reliable transfer (Layer 4)
UDP        → Fast transfer (Layer 4)
IP         → Addressing (Layer 3)
Ethernet   → LAN (Layer 2)
```

### Trick to Remember:
```
7 → All      (Application)
6 → People   (Presentation)
5 → Seem     (Session)
4 → To       (Transport)
3 → Need     (Network)
2 → Data     (Data Link)
1 → Processing (Physical)
```

---

*Notes by: IT Student*
*Topic: Computer Networks - OSI Model*
