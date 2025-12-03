# 🛡️ **Reverse Engineering – Induction Track 2**

Welcome to the second stage of the Cybersecurity Club Inductions under the **Reverse Engineering** track.

This task simulates a **small-scale ransomware analysis scenario**, designed to evaluate your RE depth, technical research skills, and your ability to think like a malware analyst.

You are given a folder containing **three items**:

```
1. static_analysis.exe
2. ransomware.exe
3. fake_imp_files/   (contains 50 dummy files)
```

Your work is divided into **two major parts**, each testing different RE skills.

---

# 📌 **Part 1 — Static Malware Analysis (30 points)**

File: **static_analysis.exe**

This binary **does NOT execute**.  
Your task is to treat it like a real malware sample used for pre-execution analysis.

You must:
1. Identify all important functions
2. Explain what each function would do in a real ransomware scenario
 3. Connect your findings to real ransomware families   
 4. Provide a research-backed workflow

### 📄 **Deliverable:**

A **detailed write-up** of your findings with screenshots.  
This section is worth **30 points**.

---

# 📌 **Part 2 — Full Ransomware Reverse Engineering Challenge (70 points)**

File: **ransomware.exe**

⚠️ **Important:**  
Run this ONLY inside the provided folder.  
Do **NOT** move it, rename it, or run it elsewhere.  
It will encrypt all files inside `fake_imp_files/`.
Disable the Windows defender in the VM.

Your goal is to **completely reverse it**, extract the key, write a decrypter, and patch the malware.

---

## 🔹 **1. Static Analysis & Offsets — 20 points**

You must analyze the binary **without running it**:

- Identify functions
    
- Understand control flow
    
- Find encryption routine
    
- Locate the key or key-generation logic
    
- Identify constants and offsets
    
- Extract strings / imports
    

Deliverables:

- Screenshots
    
- High-level function explanations
---

## 🔹 **2. Dynamic Tracing & Runtime Key Extraction — 25 points**

Now run the ransomware **in a Windows 10 or 7  VM** and observe its real behavior:

- Trace system calls
    
- Set breakpoints
    
- Capture the key from memory/registers
    
- Monitor file encryption loop
    
- Extract any runtime-only values
    

Deliverables:

- Debugger screenshots
    
- Key dump
    
- Execution trace summary
    

---

## 🔹 **3. Decrypter Correctness & Tests — 25 points**

You must build a tool that:

- Takes encrypted  files
    
- Restores them to the original format
    
- Works for all files inside `fake_imp_files/`
    

You must also verify correctness:

- Show before/after hashes
    
- Provide comparison screenshots
    
- Add sample test cases
    

---

## 🔹 **4. Binary Patch (Dry Run) — 15 points**

You must **neutralize** the ransomware by patching the binary:

Examples:

- NOP out the encryption call
    
- Patch jumps
    
- Force early exit
    
- Remove anti-debug checks
    

Deliverables:

- Patched binary
    
- Screenshot of patched instructions
    
- Explanation of offsets changed
    

---

## 🔹 **5. Final Report & Presentation — 15 points**

After completing all tasks, submit:

- A professional malware analysis report
    
- Screenshots of all stages
    
- Explanation of techniques used
    
- Lessons learned
    

This section checks clarity, structure, depth, and technical communication.

---

# 🧩 **Total Marks: 100**

|Component|Points|
|---|---|
|Static Analysis.exe Write-up|30|
|Static Analysis (Ransomware.exe)|20|
|Dynamic Analysis|25|
|Decrypter|25|
|Binary Patch|15|
|Report + Presentation|15|
|**Total**|**130** (scaled to 100)|

---

# ⚠️ **Rules & Warnings**

- Run binaries _only_ inside a controlled VM.
    
- Do not modify the folder structure.
    
- Do not upload the malware samples anywhere.
    
- No use of AI tools for solving the challenge.
    
- Your report must be original and deeply technical.
    

ALL THE BEST!!!!