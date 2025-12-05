# 📄 **Question 1 — Reverse Engineering Track Write-ups**

### _Induction Task – Month-Long Research Challenge_

Welcome to **Question 1** of the induction task.  
This section evaluates your **reverse engineering depth**, **analysis clarity**, and **ability to document complex technical work**.

You are required to complete as many modules as you can from given **five RE mini-modules** of the OST2 curriculum and then write **detailed, original write-ups** for each one.  
Each module carries **20 points**, for a total of **100 points**.
Donot forget to attempt **Task2** as well.

Your write-ups must show **your own thought process**, not just the answer.  
Copy-paste explanations or ChatGPT answers = _instant zero_.

---

# ✅ **Modules You Must Complete**

For each module listed below, complete the exercises from **[https://p.ost2.fyi/](https://p.ost2.fyi/)** and write a full analysis of what you did, how, and why.

---

## **1. Arch1001 — Assembly (20 pts)**

Your write-up should include:

- How you reversed a password check written entirely in assembly
    
- How you located and extracted a hardcoded XOR key
    
- How you reconstructed the purpose of a loop **purely from disassembly** (no symbols)
    
- How you identified the logic behind a simple “serial key generator”
    
- Reconstruction of C-like pseudocode from raw assembly
    

This module tests:  
**Instruction tracing, stack/regs tracking, mental decompilation, binary intuition.**

---

## **2. Dbg1102 — Ghidra (20 pts)**

Your write-up should describe:

- How you decompiled a stripped binary to recover the hidden password
    
- Breaking a simple custom packer layer
    
- Extracting an encrypted string table
    
- Patching a binary to print the flag
    
- Identifying algorithms (XOR loop, Base64, rotate, etc.) from decompiler output
    

This module tests:  
**Decompiler literacy, binary patching, packer analysis, static analysis skills.**

---

## **3. Dbg1012 — GDB (20 pts)**

Explain in detail:

- Using breakpoints to pause execution before strcmp and read the flag
    
- How you traced a function to locate a dynamic key generator
    
- Dumping memory regions to recover decrypted strings
    
- Overriding return values at runtime to bypass authentication
    
- Tracking hidden buffers using malloc/free breakpoints
    

This module tests:  
**Dynamic analysis, runtime manipulation, memory inspection, debugging flow.**

---

## **4. RE3011 — Reversing C++ Binaries (20 pts)**

Your write-up must include:

- Recovering class layout from mangled symbols
    
- Identifying which virtual function performs flag verification
    
- Reversing an STL-driven state machine
    
- Handling binaries with multiple interacting classes
    
- Extracting hidden data inside containers (vector/map)
    

This module tests:  
**vtable analysis, RTTI, STL reverse engineering, object-level reasoning.**

---

## **5. RE3201 — Symbolic Analysis (20 pts)**

Document your symbolic execution journey:

- How you symbolically solved for the hidden “success path”
    
- Full constraint breakdown for avoiding the failure branch
    
- Deriving the correct 4-byte key from symbolic equations
    
- Finding the shortest input triggering the deepest nested branch
    
- Solving the loop accumulator using symbolic tools instead of brute force
    

This module tests:  
**Symbolic reasoning, formal constraint solving, Z3/angr workflows.**

---

# 🧪 **Submission Requirements**

Your write-up **must include**:

### **1. Executive Summary (2–4 lines per module)**

What the challenge was _about_ (not the answer).

### **2. Tools Used**

(e.g., Ghidra, GDB, radare2, angr, pwndbg)

### **3. Step-by-Step Approach**

Show your reasoning:

- Why you looked at certain instructions
    
- Why you set specific breakpoints
    
- How you identified patterns
    
- What dead-ends you hit
    
- How you overcame them
    

### **4. Screenshots (mandatory)**

Use your own screenshots of:

- disassembly
    
- decompiler
    
- memory dumps
    
- symbolic engine constraints
    

### **5. Final Answer + Explanation**

Explain **why your solution works**, not just what it is.

---

# 🎯 **What We’re Evaluating**

We don’t care if you get everything correct.  
We care about:

- **Depth of analysis**
    
- **Clear reasoning**
    
- **Research skill**
    
- **Tool proficiency**
    
- **Documentation quality**
    

Think like a **junior malware analyst writing an internal report**.

---

# 🚫 Rules

- No copying from the internet.
    
- No AI-generated solutions (analysis must be yours).
    
- No asking for the flag/password directly.
    
- Plagiarism = **0 points and disqualification.**
    

---
