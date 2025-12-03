# Forensics tasks


## Task 1 - Malware forensics
For this assignment, you will follow the [Art of Memory Forensics](https://repo.zenk-security.com/Forensic/The%20Art%20of%20Memory%20Forensics%20-%20Detecting%20Malware%20and%20Threats%20in%20Windows,%20Linux,%20and%20Mac%20Memory%20(2014).pdf) book.

Finish the intro (Part 1) and then pick either Windows (Part II) or Linux (Part III).

## Evaluation -
1. Basics [10%] - Process and memory management, I/O,  etc.
2. Linux/Windows/Mac Internals [40%] - Memory, networking and kernel artifacts, modules, timelining, etc.
3. Proficiency of Volatility 3 and forensics tools [20%] - profiling, volshell, etc
4. Case study of real world rootkit/malware [30%] - [Babuk](https://github.com/ASm0ty/Babuk-RansomWare---October-2023) or this [one](https://github.com/Hildaboo/BabukRansomwareSourceCode/) or [LinkPro](https://vx-underground.org/Malware%20Analysis/2025/2025-10-14%20-%20LinkPro%20eBPF%20rootkit%20analysis/Samples). If you chose Windows (Part II) then pick Babuk, and if you chose Linux (Part III) pick LinkPro.

### Deliverables

A detailed report (see [one here](https://unit42.paloaltonetworks.com/thanos-ransomware/) for example, but it's got way too few details) that outlines how the malware works, and how Volatility3 was used for this. Please reference the MITRE ATT&CK framework as well. If you're doing LinkPro (Linux), then we expect you to get familiar with eBPF as well.

All code used and any memory images collected must be released publicly for assessment.


## Task 2 - Memory forensics
Imagine you're a whistleblower, and you just dropped the bomb. You sent the evidence from your phone, deleted it and then did a factory reset. Seconds later, police surround you, and they have the phone in their hands. Change perspectives; now you're a law enforcement officer who has to analyze this guy's phone. 

Model the threat in three different ways - 
1. [FDE disabled] You get the phone before the factory reset happens, and its unlocked (AFU). Assume root access as well.
2. [FDE disabled] You get the phone before the factory reset, but its shut down. 
4. [FDE enabled] You get the phone after factory reset, and the whistleblower bent, he spilled his password.

For each of this scenarios, attempt to recover the evidence file from the user's storage. Maybe it's a simple photo. Use a rooted Android, and disable FDE for 1 and 2. For 3, enable it. Bonus points if you use a jailbroken Apple device.
Yeah its hard. Document all your efforts.

## Evaluation criteria
1. Efforts (50%) - What you tried, how, etc. How good your understanding of mobile encryption process is.
2. Successs (50%) - If you succeed in any of the scenarios

## Deliverables

The dumps, and any code used
