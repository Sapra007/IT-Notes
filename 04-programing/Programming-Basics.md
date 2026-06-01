# 💻 Programming Basics - Complete Notes
> IT Student Notes | Topic: Programming Fundamentals & C Language

---

## 📌 Table of Contents
1. [Programming Kya Hai](#1-programming-kya-hai)
2. [Programming Languages](#2-programming-languages)
3. [C Language - Introduction](#3-c-language---introduction)
4. [Variables & Data Types](#4-variables--data-types)
5. [Operators](#5-operators)
6. [Input & Output](#6-input--output)
7. [Quick Revision](#7-quick-revision)

---

## 1. Programming Kya Hai

- Computer ko **instructions dena**
- Yeh instructions = **Code**
- Code likhne wala = **Programmer**
- Jis language mein code likhte hain = **Programming Language**

```
Insaan → Programming Language → Computer
(Samajh aata hai)              (0s and 1s)
```

### Levels of Language:
```
High Level    → Python, Java, C++  (Easy to write)
      ↓
Assembly      → MOV, ADD, SUB      (Medium)
      ↓
Machine Code  → 0s and 1s          (Computer samjhe)
```

---

## 2. Programming Languages

### Popular Languages:
| Language | Use |
|----------|-----|
| **C** | System programming, OS |
| **C++** | Games, System software |
| **Java** | Android, Enterprise |
| **Python** | AI/ML, Data Science ✅ |
| **JavaScript** | Web development |
| **SQL** | Database |
| **PHP** | Web backend |

### C Language se Kyun Shuru Karein:
```
✅ Sabse basic language
✅ Computer ka kaam samajh aata hai
✅ Memory management sikhte hain
✅ Baaki languages easy lagti hain baad mein
✅ IT exams mein C zaroori hai
```

### Compiled vs Interpreted:
| | Compiled | Interpreted |
|--|----------|-------------|
| Example | C, C++ | Python, JS |
| Translation | Pehle poora | Line by line |
| Speed | Fast ✅ | Thoda slow |
| Error | Baad mein | Turant |

---

## 3. C Language - Introduction

### Pehla Program:
```c
#include <stdio.h>

int main() {
    printf("Hello World!\n");
    return 0;
}
```

### Har Line Ka Matlab:
```c
#include <stdio.h>   → stdio library include karo
                       (Input/Output functions ke liye)

int main()           → Program yahan se shuru hota hai
                       (main function)

{  }                 → Code block shuru aur khatam

printf("Hello!")     → Screen pe print karo

\n                   → New line

return 0             → Program successfully khatam
```

### C Program Structure:
```c
// 1. Header Files
#include <stdio.h>
#include <stdlib.h>

// 2. Main Function
int main() {

    // 3. Variables declare karo
    int age = 20;

    // 4. Logic likho
    printf("Age: %d", age);

    // 5. Return
    return 0;
}
```

### Comments:
```c
// Yeh single line comment hai

/* Yeh
   multi line
   comment hai */
```

---

## 4. Variables & Data Types

### Variable kya hota hai:
```
Variable = Data store karne ki jagah
Jaise ek dabba jisme kuch rakho!

int age = 20;
 ↑    ↑    ↑
Type Name Value
```

### Data Types:
| Type | Matlab | Size | Example |
|------|--------|------|---------|
| **int** | Whole number | 4 bytes | 1, 2, 100 |
| **float** | Decimal number | 4 bytes | 3.14, 2.5 |
| **double** | Big decimal | 8 bytes | 3.14159265 |
| **char** | Single character | 1 byte | 'A', 'z' |

### Examples:
```c
int age = 20;
float marks = 85.5;
double pi = 3.14159265;
char grade = 'A';
```

### Variable Rules:
```
✅ Letters, numbers, underscore use kar sakte ho
✅ Letter ya underscore se shuru hona chahiye
❌ Number se shuru nahi kar sakte
❌ Spaces allowed nahi
❌ Keywords use nahi kar sakte (int, float, etc.)

Valid:   age, my_name, marks2
Invalid: 2marks, my name, int
```

### Constants:
```c
// Value change nahi hogi
const float PI = 3.14;
const int MAX = 100;
```

---

## 5. Operators

### Arithmetic Operators:
| Operator | Kaam | Example | Result |
|----------|------|---------|--------|
| + | Addition | 5 + 3 | 8 |
| - | Subtraction | 5 - 3 | 2 |
| * | Multiplication | 5 * 3 | 15 |
| / | Division | 10 / 2 | 5 |
| % | Remainder (Modulus) | 10 % 3 | 1 |

### Comparison Operators:
| Operator | Kaam | Example | Result |
|----------|------|---------|--------|
| == | Equal to | 5 == 5 | True |
| != | Not equal | 5 != 3 | True |
| > | Greater than | 5 > 3 | True |
| < | Less than | 5 < 3 | False |
| >= | Greater or equal | 5 >= 5 | True |
| <= | Less or equal | 3 <= 5 | True |

### Logical Operators:
| Operator | Kaam | Example |
|----------|------|---------|
| && | AND - dono true hone chahiye | a > 0 && b > 0 |
| \|\| | OR - ek true ho toh chalega | a > 0 \|\| b > 0 |
| ! | NOT - ulta kar do | !(a > 0) |

### Assignment Operators:
```c
int a = 10;    // a = 10
a += 5;        // a = a + 5 = 15
a -= 3;        // a = a - 3 = 12
a *= 2;        // a = a * 2 = 24
a /= 4;        // a = a / 4 = 6
a %= 4;        // a = a % 4 = 2
```

### Increment/Decrement:
```c
int a = 5;
a++;    // a = 6 (increment)
a--;    // a = 5 (decrement)
++a;    // pehle increment phir use
a++;    // pehle use phir increment
```

---

## 6. Input & Output

### Output - printf():
```c
printf("Hello!");                    // Simple text
printf("Age: %d", age);             // Integer
printf("Marks: %f", marks);         // Float
printf("Grade: %c", grade);         // Character
printf("Name: %s", name);           // String
printf("Age: %d, Marks: %f", age, marks); // Multiple
```

### Input - scanf():
```c
int age;
scanf("%d", &age);          // Integer input

float marks;
scanf("%f", &marks);        // Float input

char grade;
scanf("%c", &grade);        // Character input
```

### Format Specifiers:
| Specifier | Data Type |
|-----------|-----------|
| %d | int |
| %f | float |
| %lf | double |
| %c | char |
| %s | string |

### Escape Sequences:
| Sequence | Matlab |
|----------|--------|
| \n | New line |
| \t | Tab space |
| \\ | Backslash |
| \" | Double quote |

### Example Program:
```c
#include <stdio.h>

int main() {
    int age;
    float marks;

    printf("Apni age enter karo: ");
    scanf("%d", &age);

    printf("Apne marks enter karo: ");
    scanf("%f", &marks);

    printf("\nTumhari age: %d\n", age);
    printf("Tumhare marks: %.2f\n", marks);

    return 0;
}
```

---

## 7. Quick Revision

```
Programming  = Computer ko instructions dena
Variable     = Data store karne ki jagah
Data Type    = Variable ka type (int, float, char)
Operator     = Calculation ya comparison karna
printf()     = Screen pe print karna
scanf()      = User se input lena
%d           = int format specifier
%f           = float format specifier
%c           = char format specifier
\n           = New line
```

### C Program Structure:
```c
#include <stdio.h>      // Header

int main() {            // Main function
    // Variables
    // Logic
    // Input/Output
    return 0;           // End
}
```

### Data Types Summary:
```
int    → 4 bytes → Whole numbers
float  → 4 bytes → Decimal numbers
double → 8 bytes → Big decimal numbers
char   → 1 byte  → Single character
```

---

*Notes by: IT Student*
*Topic: Programming Basics - Introduction & C Language*
