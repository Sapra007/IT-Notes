# 💻 Software & Operating System - Complete Notes
> IT Student Notes | Topic: Software Fundamentals & OS

---

## 📌 Table of Contents
1. [Software Kya Hai](#1-software-kya-hai)
2. [Software ke Types](#2-software-ke-types)
3. [System Software](#3-system-software)
4. [Application Software](#4-application-software)
5. [Programming Software](#5-programming-software)
6. [Operating System - Deep Dive](#6-operating-system---deep-dive)
7. [OS ke Main Functions](#7-os-ke-main-functions)
8. [Popular OS Comparison](#8-popular-os-comparison)
9. [Boot Process](#9-boot-process)
10. [Kernel](#10-kernel)
11. [Quick Revision](#11-quick-revision)

---

## 1. Software Kya Hai

- Software **instructions ka set** hai
- Computer ko batata hai **kya karna hai**
- Hardware ke bina software kaam nahi kar sakta
- Software ke bina hardware sirf ek **"box"** hai!

### Hardware vs Software:

| Hardware | Software |
|----------|---------|
| Physical parts | Instructions |
| 🖥️ Monitor | 👁️ Display Driver |
| ⌨️ Keyboard | ⌨️ Keyboard Driver |
| 🧠 CPU | 🔄 Operating System |
| 💾 RAM | 📦 Applications |

---

## 2. Software ke Types

```
SOFTWARE
│
├── 1. System Software
│   ├── Operating System
│   ├── Device Drivers
│   └── Utilities
│
├── 2. Application Software
│   ├── General Purpose
│   ├── Specific Purpose
│   └── Web Based
│
└── 3. Programming Software
    ├── Compilers
    ├── Interpreters
    └── IDEs
```

---

## 3. System Software

- Computer ko **chalane** ke liye zaroori hai
- User directly use nahi karta
- Background mein kaam karta hai

### Types:

| Type | Kaam | Example |
|------|------|---------|
| **Operating System** | Sab manage karta hai | Windows, Linux |
| **Device Drivers** | Hardware ko control karta hai | Printer driver, GPU driver |
| **Utilities** | System maintain karta hai | Antivirus, Disk cleaner |

---

## 4. Application Software

- User directly use karta hai
- Specific kaam ke liye bana hota hai

### General Purpose:

| App | Kaam |
|-----|------|
| MS Word | Document banana |
| Excel | Spreadsheet |
| Chrome | Internet browse |
| VLC | Video play |

### Specific Purpose:

| App | Kaam |
|-----|------|
| Tally | Accounting |
| AutoCAD | Engineering design |
| Photoshop | Photo editing |
| VS Code | Coding ✅ |

### Web Based:

| App | Kaam |
|-----|------|
| Gmail | Email |
| Google Docs | Online documents |
| YouTube | Videos |
| ChatGPT | AI assistant |

---

## 5. Programming Software

### Compiler
- Poora code ek saath **translate** karta hai
- Example: C, C++

```
Source Code → [COMPILER] → Machine Code
(Human readable)           (Computer readable)
```

### Interpreter
- Code **line by line** translate karta hai
- Example: Python, JavaScript

```
Line 1 → Execute
Line 2 → Execute
Line 3 → Execute
```

### Compiler vs Interpreter:

| | Compiler | Interpreter |
|--|----------|-------------|
| Translation | Poora ek saath | Line by line |
| Speed | Fast | Thoda slow |
| Error | Baad mein batata hai | Turant batata hai |
| Example | C, C++ | Python, JS |

### IDE (Integrated Development Environment):

| IDE | Language |
|-----|---------|
| VS Code | Sab kuch ✅ |
| PyCharm | Python |
| Eclipse | Java |
| IntelliJ | Java, Kotlin |

---

## 6. Operating System - Deep Dive

- OS ka full form = **Operating System**
- Hardware aur user ke beech **bridge** hai
- Computer ka **"backbone software"** hai
- Bina OS ke computer **useless** hai!

### OS ka Structure:

```
USER
 ↕
APPLICATIONS (Chrome, Word, Games)
 ↕
OPERATING SYSTEM ← (Manager)
 ↕
HARDWARE (CPU, RAM, Storage)
```

### Popular OS:

| OS | Use |
|----|-----|
| Windows | Personal PC, Office |
| Linux | Servers, Programming ✅ |
| macOS | Apple computers |
| Android | Mobile |
| iOS | iPhone |

### Open Source vs Closed Source:

| | Open Source | Closed Source |
|--|-------------|---------------|
| Code | Sabko milta hai | Secret |
| Price | Free | Paid |
| Example | Linux, Firefox | Windows, Photoshop |
| Modify | Kar sakte ho ✅ | Nahi |

---

## 7. OS ke Main Functions

### 1. 🧠 Process Management

#### Process kya hota hai?
- Jab koi program run hota hai → **Process** ban jaata hai
- Example: Chrome open kiya → Chrome ek process hai

```
Program (Disk pe) → Run kiya → Process (RAM mein)
Chrome.exe → Double click → Chrome Process
```

#### Process ke States:
```
NEW → READY → RUNNING → WAITING → TERMINATED
```

| State | Matlab |
|-------|--------|
| New | Process ban rahi hai |
| Ready | CPU ka wait kar rahi hai |
| Running | CPU use kar rahi hai |
| Waiting | Kisi cheez ka wait |
| Terminated | Khatam ho gayi |

#### CPU Scheduling:
- Ek CPU = ek baar mein **ek hi process**
- OS decide karta hai kaunsi process pehle chalegi

```
Process Queue:
[Chrome] [Word] [Game] [Music]
              ↓
         CPU Scheduler
              ↓
    Ek ek karke sab chalata hai
    Itni fast ki lagta hai sab ek saath chal rahe hain!
```

---

### 2. 💾 Memory Management

#### OS RAM kaise manage karta hai:
```
RAM (8GB total)
┌─────────────────────┐
│ OS itself (1GB)     │
├─────────────────────┤
│ Chrome (2GB)        │
├─────────────────────┤
│ Word (500MB)        │
├─────────────────────┤
│ Game (3GB)          │
├─────────────────────┤
│ Free Space (1.5GB)  │
└─────────────────────┘
```

#### Virtual Memory:
- RAM full ho gayi? OS **HDD/SSD ka kuch hissa** RAM ki tarah use karta hai
- Isko **Virtual Memory** kehte hain

```
RAM (8GB) + Virtual Memory (HDD se 4GB) = 12GB jaisi feel
⚠️ But yeh slow hota hai!
```

---

### 3. 📁 File Management

#### File System kya hota hai?
- OS files ko **organize** karta hai
- Folders aur files ka structure maintain karta hai

```
C:/
│
├── Windows/
│   ├── System32/
│   └── Users/
│
├── Program Files/
│   ├── Chrome/
│   └── Office/
│
└── Users/
    └── YourName/
        ├── Desktop/
        ├── Documents/
        └── Downloads/
```

#### File Systems ke Types:

| File System | OS | Feature |
|-------------|-----|---------|
| NTFS | Windows | Secure, large files ✅ |
| FAT32 | Old Windows | Simple, small files |
| ext4 | Linux | Fast, reliable ✅ |
| APFS | macOS | Apple optimized |

---

### 4. 🔒 Security Management

```
✅ User Authentication  → Password, PIN, Fingerprint
✅ Permissions          → Kaun kya access kar sakta hai
✅ Firewall             → Network security
✅ Encryption           → Data protect karna
✅ Updates              → Security patches
```

#### User Permissions:

```
ADMIN (Full access)
├── Install software ✅
├── Delete system files ✅
└── Change settings ✅

NORMAL USER (Limited access)
├── Install software ❌
├── Delete system files ❌
└── Change settings ❌ (mostly)
```

---

### 5. 🔌 Device Management

#### Driver kya hota hai?
- Har hardware device ka ek **driver** hota hai
- Driver OS ko batata hai device kaise use karein

```
Printer lagaya
      ↓
OS ne puchha: "Yeh kya hai?"
      ↓
Driver ne bataya: "Main printer hoon!"
      ↓
Ab OS printer use kar sakta hai ✅
```

---

### 6. 🖥️ User Interface (UI)

#### CLI (Command Line Interface):
- Text commands type karte hain
- Example: Linux Terminal, CMD

```bash
$ ls          → files list karo
$ cd folder   → folder mein jao
$ mkdir test  → folder banao
$ rm file.txt → file delete karo
```

#### GUI (Graphical User Interface):
- Mouse se click karte hain
- Icons, buttons, windows hote hain
- Example: Windows, macOS

| | CLI | GUI |
|--|-----|-----|
| Use | Commands type karo | Mouse se click karo |
| Speed | Fast | Thoda slow |
| Difficulty | Technical | Easy |
| Use Case | Servers, Programming | Normal users |

---

## 8. Popular OS Comparison

| Feature | Windows | Linux | macOS |
|---------|---------|-------|-------|
| Price | Paid | Free ✅ | Paid |
| Security | Average | Best ✅ | Good |
| Gaming | Best ✅ | Average | Poor |
| Programming | Good | Best ✅ | Good |
| User Friendly | Best ✅ | Average | Good |
| Servers | Average | Best ✅ | Average |

---

## 9. Boot Process

```
1. Power ON
      ↓
2. BIOS/UEFI chalu hota hai
      ↓
3. POST (Hardware Check)
   CPU ✅ RAM ✅ Storage ✅
      ↓
4. Bootloader dhundta hai
      ↓
5. OS load hota hai (RAM mein)
      ↓
6. Login screen aati hai
      ↓
7. Desktop load hota hai ✅
```

> **POST** = Power On Self Test

---

## 10. Kernel

- OS ka **sabse important** aur core part
- Hardware aur software ke beech directly kaam karta hai

```
USER APPLICATIONS
      ↕
   KERNEL ← (Core of OS)
      ↕
   HARDWARE
```

### Kernel ke Kaam:
```
✅ Process manage karna
✅ Memory manage karna
✅ Hardware se communicate karna
✅ Security ensure karna
```

### Kernel ke Types:

| Type | Feature | Example |
|------|---------|---------|
| **Monolithic** | Sab ek jagah | Linux |
| **Microkernel** | Alag alag parts | macOS |
| **Hybrid** | Dono ka mix | Windows |

---

## 11. Quick Revision

### Software Types Summary:
```
🔧 System Software     → OS, Drivers, Utilities
📱 Application Software → Word, Chrome, Games
👨‍💻 Programming Software → Compiler, IDE, Interpreter
```

### OS Functions Summary:
```
🧠 Process Management  → Programs chalana, CPU schedule
💾 Memory Management   → RAM allocate karna
📁 File Management     → Files organize karna
🔒 Security            → Users aur data protect karna
🔌 Device Management   → Hardware drivers
🖥️ User Interface      → CLI ya GUI
```

### Important Definitions:
```
Process   = Running program
Kernel    = OS ka core
Driver    = Hardware ko OS se connect karta hai
CLI       = Text based interface
GUI       = Graphical interface
Virtual Memory = HDD ko RAM ki tarah use karna
File System    = Files organize karne ka tarika
```

---

### Analogy:
```
🏢 Company (Computer)
│
├── 👔 CEO (Kernel)          → Sab control karta hai
├── 👥 Employees (Processes) → Kaam karte hain
├── 🗂️ Filing (File Mgmt)    → Documents organize
├── 💰 Budget (Memory Mgmt)  → Resources allocate
└── 🔒 Security Guard        → Security manage
```

---

*Notes by: IT Student*
*Topic: Software Introduction & Operating System*
