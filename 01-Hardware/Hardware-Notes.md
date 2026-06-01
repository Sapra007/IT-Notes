# 💻 Computer Hardware - Complete Notes
> IT Student Notes | Topic: Hardware Fundamentals

---

## 📌 Table of Contents
1. [Computer Kya Hai](#1-computer-kya-hai)
2. [CPU - Central Processing Unit](#2-cpu---central-processing-unit)
3. [RAM - Random Access Memory](#3-ram---random-access-memory)
4. [Storage - HDD & SSD](#4-storage---hdd--ssd)
5. [Motherboard](#5-motherboard)
6. [GPU - Graphics Processing Unit](#6-gpu---graphics-processing-unit)
7. [PSU - Power Supply Unit](#7-psu---power-supply-unit)
8. [Input/Output Devices](#8-inputoutput-devices)
9. [Networking Hardware](#9-networking-hardware)

---

## 1. Computer Kya Hai

Computer ek **electronic device** hai jo:
- **Input** leta hai
- **Process** karta hai
- **Output** deta hai

### Main Components:
| Component | Kaam |
|-----------|------|
| CPU | Processing (Brain) |
| RAM | Temporary Memory |
| Storage | Permanent Memory |
| Motherboard | Sab ko connect karta hai |
| GPU | Graphics handle karta hai |
| PSU | Power deta hai |

### Simple Flow:
```
Input → CPU (Process) → Output
           ↕
      RAM + Storage
```

---

## 2. CPU - Central Processing Unit

- Computer ka **"Brain"** hai
- Saari calculations aur processing karta hai
- Example: Intel Core i5, AMD Ryzen 5

### CPU ke andar:

| Part | Kaam |
|------|------|
| **ALU** (Arithmetic Logic Unit) | Math aur Logic calculations |
| **CU** (Control Unit) | Baaki parts ko instructions deta hai |
| **Registers** | CPU ke andar ki fastest memory |
| **Cache (L1/L2/L3)** | RAM se fast temporary memory |

### CPU ka Fetch-Decode-Execute Cycle:
```
Step 1: FETCH   → Instruction RAM se uthao
Step 2: DECODE  → Samjho ki kya karna hai
Step 3: EXECUTE → Kaam karo (ALU use karo)
Step 4: STORE   → Result save karo
```
> Yeh cycle **billions of times per second** hoti hai!

### Important CPU Terms:

| Term | Matlab |
|------|--------|
| **Clock Speed** | GHz mein, jitni zyada = utna fast |
| **Cores** | Ek CPU mein kitne "brains" hain |
| **Threads** | Ek core kitne kaam ek saath kar sakta hai |
| **64-bit** | Ek baar mein kitna data process ho sakta hai |

### Example:
> Intel Core i5 - 12th Gen, 6 Cores, 12 Threads, 3.7GHz
> - 6 Cores = 6 kaam ek saath
> - 12 Threads = 12 tasks handle
> - 3.7GHz = 3.7 billion cycles/second

---

## 3. RAM - Random Access Memory

- **Temporary memory** hai (Volatile)
- Computer ki **"short term memory"**
- Power off = Data delete!

### RAM kaam kaise karta hai:
```
HDD/SSD (Permanent)
      ↓
   RAM (Temporary) ←→ CPU (Processing)
```
> CPU directly HDD se data nahi leta, pehle RAM mein aata hai!

### RAM ke Types:

| Type | Feature |
|------|---------|
| **DRAM** | Common, baar baar refresh hoti hai |
| **SRAM** | Cache mein use, bahut fast |
| **DDR3** | Purani generation |
| **DDR4** | Common, fast |
| **DDR5** | Latest, bahut fast |

### RAM Capacity:

| RAM | Use |
|-----|-----|
| 4GB | Basic, slow |
| 8GB | Normal use |
| 16GB | Gaming, Coding ✅ |
| 32GB+ | Video editing, Servers |

### RAM vs Storage:

| | RAM | Storage |
|--|-----|---------|
| Type | Temporary | Permanent |
| Speed | Bahut Fast | Slow/Fast |
| Data on Power Off | Delete | Save |
| Size | 4-64GB | 256GB-4TB |

### Analogy:
```
📚 Almari (HDD/SSD) = Permanent storage
🗂️ Desk (RAM)       = Jo abhi kaam kar rahe ho
🧠 Dimag (CPU)      = Processing
```

---

## 4. Storage - HDD & SSD

Storage = **Permanent Memory** (Data save rehta hai)

---

### HDD (Hard Disk Drive)

- Andar **mechanical parts** hote hain
- Magnetic disk ghoomti hai (5400-7200 RPM)
- Read/Write head data access karta hai

| Feature | Detail |
|---------|--------|
| Speed | Slow (100-150 MB/s) |
| Price | Sasta |
| Capacity | 1TB - 10TB+ |
| Durability | Mechanical, toot sakta hai |

---

### SSD (Solid State Drive)

- **Koi moving parts nahi**
- Flash memory chips use karta hai
- Pen drive jaisa kaam karta hai

| Feature | Detail |
|---------|--------|
| Speed | Fast (500-7000 MB/s) |
| Price | Thoda mehnga |
| Capacity | 256GB - 4TB |
| Durability | Zyada strong |

---

### HDD vs SSD:

| | HDD | SSD |
|--|-----|-----|
| Speed | Slow 🐢 | Fast 🚀 |
| Price | Sasta | Mehnga |
| Moving Parts | Haan | Nahi |
| Best For | Bulk storage | OS, Programs |

---

### Aur Storage Types:

| Type | Use |
|------|-----|
| USB Flash Drive | Portable storage |
| SD Card | Camera, Phone |
| Cloud Storage | Google Drive, OneDrive |
| Optical (CD/DVD) | Purana, ab rare |

### Storage Units:
```
8 Bits      = 1 Byte
1024 Bytes  = 1 KB (Kilobyte)
1024 KB     = 1 MB (Megabyte)
1024 MB     = 1 GB (Gigabyte)
1024 GB     = 1 TB (Terabyte)
1024 TB     = 1 PB (Petabyte)
```

---

## 5. Motherboard

- Computer ka **"Backbone"** hai
- Saare components isse connected hote hain
- Bina motherboard ke koi part kaam nahi kar sakta

### Motherboard ke Parts:

| Part | Kaam |
|------|------|
| **CPU Socket** | CPU yahan lagta hai |
| **RAM Slots** | RAM yahan lagti hai |
| **PCIe Slots** | GPU aur cards yahan lagte hain |
| **SATA Ports** | HDD/SSD connect hote hain |
| **Power Connector** | PSU se power aati hai |
| **BIOS Chip** | Computer start hone pe pehle chalta hai |
| **Heatsink Connectors** | CPU fan yahan lagta hai |

### Back Panel Ports:

| Port | Kaam |
|------|------|
| USB | Pen drive, Mouse, Keyboard |
| HDMI/DisplayPort | Monitor connect karna |
| LAN (Ethernet) | Internet cable |
| Audio Jack | Headphone, Speaker |

### Motherboard Sizes (Form Factor):

| Size | Naam | Use |
|------|------|-----|
| Sabse bada | ATX | Normal PC |
| Medium | Micro-ATX | Compact PC |
| Chota | Mini-ITX | Small PC |

### BIOS Boot Process:
```
Power ON → BIOS chalu → Hardware Check
→ Bootloader → OS Load → Login Screen ✅
```

### Motherboard Choose Karte Waqt:
- CPU Socket match hona chahiye
- RAM DDR4 ya DDR5 support
- Size (ATX/Micro-ATX)
- Ports kitne chahiye

---

## 6. GPU - Graphics Processing Unit

- **Graphics/Visuals** handle karta hai
- Games, videos, animations sab GPU karta hai

### CPU vs GPU:

| | CPU | GPU |
|--|-----|-----|
| Cores | Few powerful (4-16) | Thousands of small |
| Tasks | Serial | Parallel |
| Use | General purpose | Graphics specific |

### GPU ke 2 Types:

| Type | Feature |
|------|---------|
| **Integrated GPU** | CPU ke andar, weak, basic kaam |
| **Dedicated GPU** | Alag card, powerful, gaming/AI |

### GPU ke Parts:

| Part | Kaam |
|------|------|
| **CUDA Cores** (NVIDIA) | GPU ke workers |
| **Stream Processors** (AMD) | GPU ke workers |
| **VRAM** | GPU ki apni RAM |
| **Cooling System** | Heat manage karta hai |

### VRAM:

| VRAM | Use |
|------|-----|
| 4GB | Basic gaming |
| 8GB | Normal gaming ✅ |
| 12GB+ | 4K gaming, AI/ML |

### Popular GPUs:

| Brand | Budget | Mid | High End |
|-------|--------|-----|----------|
| NVIDIA | GTX 1650 | RTX 3060 | RTX 4090 |
| AMD | RX 6600 | RX 7700 XT | RX 7900 XTX |

### GPU Use Cases:
- 🎮 Gaming
- 🎬 Video Editing
- 🤖 AI / Machine Learning
- 🎨 3D Rendering
- ⛏️ Crypto Mining

---

## 7. PSU - Power Supply Unit

- Computer ka **"Heart"** hai
- AC power ko DC mein convert karta hai
- Bina PSU ke koi part kaam nahi karega!

### AC vs DC:

| | AC | DC |
|--|----|----|
| Source | Wall socket | PSU, Battery |
| Computer use | Nahi | Haan ✅ |

### PSU ke Voltages:
```
+12V → CPU, GPU (Sabse important)
+5V  → USB, Storage
+3.3V → RAM, Motherboard
```

### Wattage Guide:

| Wattage | Use |
|---------|-----|
| 450W | Basic PC, no GPU |
| 550W | Normal Gaming |
| 650W | Mid range GPU ✅ |
| 750W+ | High end GPU |
| 1000W+ | Extreme/Workstation |

### Wattage Calculate Kaise Karein:
```
CPU + GPU + RAM + Storage + Extra = Total
Add 20% buffer = Final PSU wattage
```

### 80 PLUS Efficiency Rating:

| Rating | Efficiency |
|--------|-----------|
| Standard | 80% |
| Bronze | 82% |
| Silver | 85% |
| Gold | 87% ✅ Best Value |
| Platinum | 90% |
| Titanium | 92% |

### PSU Connectors:

| Connector | Kaam |
|-----------|------|
| 24-pin | Motherboard |
| 8-pin CPU | CPU |
| PCIe 6+2 pin | GPU |
| SATA | HDD/SSD |

### PSU Types:

| Type | Feature |
|------|---------|
| Non-Modular | Fixed cables, sasta, messy |
| Modular | Removable cables, clean ✅ |

### PSU Kharab Hone ke Signs:
- Computer randomly band ho jaata hai
- Burning smell aata hai
- PC start nahi hota
- Weird sounds aate hain

---

## 8. Input/Output Devices

### Input Devices (Data andar bhejte hain):

| Device | Kaam |
|--------|------|
| **Keyboard** | Text input |
| **Mouse** | Pointer control |
| **Microphone** | Sound input |
| **Camera/Webcam** | Image/Video input |
| **Scanner** | Physical doc → Digital |
| **Joystick/Gamepad** | Gaming |
| **Barcode Scanner** | Barcode read karna |

### Keyboard Types:

| Type | Feature |
|------|---------|
| Membrane | Normal, sasta |
| Mechanical | Clickable, gaming ✅ |
| Wireless | Bluetooth |
| Virtual | Touch screen pe |

### Mouse DPI:
```
DPI = Dots Per Inch
Normal use → 800-1200 DPI
Gaming     → 3200+ DPI
```

---

### Output Devices (Data bahar dete hain):

| Device | Kaam |
|--------|------|
| **Monitor** | Visual output |
| **Printer** | Physical print |
| **Speakers** | Audio output |
| **Projector** | Badi screen display |
| **Plotter** | Large engineering drawings |

### Monitor Specs:

| Resolution | Quality |
|-----------|---------|
| 1280x720 | HD |
| 1920x1080 | Full HD ✅ |
| 2560x1440 | QHD |
| 3840x2160 | 4K |

| Refresh Rate | Use |
|-------------|-----|
| 60Hz | Normal |
| 144Hz | Gaming ✅ |
| 240Hz | Pro Gaming |

### Printer Types:

| Type | Use |
|------|-----|
| Inkjet | Colors, Photos |
| Laser | Fast, Office ✅ |
| 3D Printer | 3D objects |
| Thermal | Receipts |

### Input + Output Both:

| Device | Input | Output |
|--------|-------|--------|
| Touch Screen | Touch | Display |
| Headset | Mic | Audio |
| USB Drive | Store | Retrieve |

---

## 9. Networking Hardware

Network = Do ya zyada computers jo ek dusre se connected hain

### Main Networking Devices:

| Device | Kaam |
|--------|------|
| **NIC** | Computer ko network se connect karta hai |
| **Switch** | Multiple computers ko ek network mein connect karta hai |
| **Router** | Networks ko connect, internet share karta hai |
| **Modem** | ISP se internet connection leta hai |
| **Access Point** | WiFi signal extend karta hai |
| **Repeater** | Signal boost karta hai |

### Switch vs Hub:

| | Switch | Hub |
|--|--------|-----|
| Data | Sirf sahi device ko | Sabko |
| Speed | Fast ✅ | Slow |
| Use | Aajkal | Obsolete |

### Network Flow:
```
Internet (ISP) → Modem → Router → Switch → PC
                              ↓
                           WiFi Devices
```

### IP Address:
```
Har device ka unique address = IP Address
IPv4 → 192.168.1.1 (Common)
IPv6 → 2001:0db8:85a3::8a2e:0370:7334 (Naya)
```

### MAC Address:
```
Har NIC ka unique address
Example: 00:1A:2B:3C:4D:5E
Jaise Aadhar number!
```

### Network Types:

| Type | Full Form | Range |
|------|-----------|-------|
| PAN | Personal Area Network | 10 meter (Bluetooth) |
| LAN | Local Area Network | Ek building/ghar |
| MAN | Metropolitan Area Network | Ek shehar |
| WAN | Wide Area Network | Poori duniya |

### Cables:

| Cable | Speed |
|-------|-------|
| Cat5e | 1 Gbps |
| Cat6 | 10 Gbps ✅ |
| Fiber Optic | Bahut fast, long distance |

---

## 📝 Quick Revision - Hardware Summary

```
🧠 CPU        → Brain, processing karta hai
💾 RAM        → Temporary memory, fast
📦 Storage    → Permanent memory, HDD/SSD
🟢 Motherboard → Backbone, sab connected
🎮 GPU        → Graphics handle karta hai
⚡ PSU        → Power deta hai, AC→DC
⌨️ Input      → Data andar (Keyboard, Mouse)
🖥️ Output     → Data bahar (Monitor, Printer)
🌐 Network    → Devices connect karta hai
```

---

*Notes by: IT Student*
*Topic: Computer Hardware Fundamentals*
