# 🌐 Computer Networks - Basics
> IT Student Notes | Topic: Network Fundamentals

---

## 📌 Table of Contents
1. [Network Kya Hai](#1-network-kya-hai)
2. [Network ke Types](#2-network-ke-types)
3. [Network Topologies](#3-network-topologies)
4. [Transmission Media](#4-transmission-media)
5. [Quick Revision](#5-quick-revision)

---

## 1. Network Kya Hai

- Do ya zyada computers jo **ek dusre se connected** hain
- Data aur resources **share** kar sakte hain
- Internet bhi ek **bahut bada network** hai!

### Data kaise travel karta hai:
```
Tumhara PC → Network Device → Internet → Website
     ↑                                      ↓
     └──────────── Response ────────────────┘
```

---

## 2. Network ke Types

| Type | Full Form | Range | Example |
|------|-----------|-------|---------|
| **PAN** | Personal Area Network | 10 meter | Bluetooth |
| **LAN** | Local Area Network | Ek building | Office, Ghar |
| **MAN** | Metropolitan Area Network | Ek shehar | City network |
| **WAN** | Wide Area Network | Poori duniya | Internet |

---

## 3. Network Topologies

Topology = Network mein computers **kaise connected** hain

---

### 1. 🔵 Bus Topology
```
PC1 --- PC2 --- PC3 --- PC4
        (Ek hi cable)
```
| Feature | Detail |
|---------|--------|
| Structure | Sabse simple |
| Drawback | Ek cable toot gayi = sab band ❌ |
| Use | Purana, ab rare |

---

### 2. ⭐ Star Topology
```
      PC1
       |
PC4 - Switch - PC2
       |
      PC3
```
| Feature | Detail |
|---------|--------|
| Structure | Sab switch se connected |
| Advantage | Ek PC kharab = baaki theek ✅ |
| Drawback | Switch kharab = sab band |
| Use | Sabse common aajkal ✅ |

---

### 3. 🔄 Ring Topology
```
PC1 → PC2 → PC3 → PC4 → PC1
```
| Feature | Detail |
|---------|--------|
| Structure | Circle mein connected |
| Drawback | Ek PC kharab = sab affected ❌ |
| Use | Kam use hota hai |

---

### 4. 🕸️ Mesh Topology
```
PC1 ←→ PC2
 ↕  ✕   ↕
PC3 ←→ PC4
```
| Feature | Detail |
|---------|--------|
| Structure | Sab se sab connected |
| Advantage | Bahut reliable ✅ |
| Drawback | Mehnga aur complex |
| Use | Military, Critical systems |

---

### Topology Comparison:

| Topology | Cost | Reliability | Speed | Use |
|----------|------|-------------|-------|-----|
| Bus | Sasta | Kam | Slow | Purana |
| Star | Medium | Achha ✅ | Fast | Common ✅ |
| Ring | Medium | Average | Medium | Rare |
| Mesh | Mehnga | Best ✅ | Best | Critical |

---

## 4. Transmission Media

### Wired (Cable se):

| Cable | Speed | Use |
|-------|-------|-----|
| **Cat5e** | 1 Gbps | Normal LAN |
| **Cat6** | 10 Gbps | Fast LAN ✅ |
| **Cat6a** | 10 Gbps+ | Advanced LAN |
| **Fiber Optic** | 100+ Gbps | Long distance |

#### Fiber Optic kaise kaam karta hai:
```
Normal Cable → Electricity se data travel
Fiber Optic  → Light se data travel 🚀
              (Bahut fast!)
```

---

### Wireless (Bina cable ke):

| Type | Speed | Range | Use |
|------|-------|-------|-----|
| **WiFi 5** | 3.5 Gbps | 35m | Normal |
| **WiFi 6** | 9.6 Gbps | 35m | Latest ✅ |
| **Bluetooth** | 3 Mbps | 10m | PAN |
| **4G** | 150 Mbps | km tak | Mobile |
| **5G** | 10 Gbps | km tak | Future ✅ |

---

### Wired vs Wireless:

| | Wired | Wireless |
|--|-------|---------|
| Speed | Fast ✅ | Thoda slow |
| Security | Better ✅ | Weak |
| Mobility | Nahi | Haan ✅ |
| Setup | Complex | Easy |
| Cost | Zyada | Kam |

---

## 5. Quick Revision

```
🌐 Network    = Computers ka connected group
📍 PAN        = Bluetooth (10m)
🏠 LAN        = Ghar/Office (1 building)
🏙️ MAN        = Ek shehar
🌍 WAN        = Poori duniya (Internet)

🔵 Bus        = Simple, ek cable, unreliable
⭐ Star       = Common, switch based ✅
🔄 Ring       = Circle, ek fail = sab fail
🕸️ Mesh       = Sab connected, reliable, mehnga

🔌 Wired      = Fast, secure, Cat6/Fiber
📡 Wireless   = Mobile, easy, WiFi/5G
```

---

*Notes by: IT Student*
*Topic: Computer Networks - Basics*
