# Cryptography Tasks (Track 2)

This document outlines the tasks and expectations for prospective inductees interested in the Cryptography domain. We have designed these challenges to gauge your aptitude for both, the mathematical foundations of cryptography and its practical application in capturing flags (CTFs).  

To be considered for induction, you are required to attempt either one of the following two tasks. We do not expect perfection; we are looking for curiosity, persistence, and a willingness to learn complex topics.

## Note

Don't panic if you cannot finish everything.

Cryptography is a dense field, and this is a challenging list. We are looking for potential, not experts. If you get stuck on the Lattice challenges or find the textbook proofs difficult, focus on what you can understand and be ready to discuss your partial efforts. A solid attempt at learning difficult material is worth more to us than a completed checklist with no understanding.  

Good luck!

## Task 1: Practical Challenge - The CryptoHack Lattice Course

### Objective:

Gain hands-on experience with lattice-based cryptography, a critical area for modern and post-quantum security.

### Action:

Register on CryptoHack and complete all challenges (Lattices, LWE1 and LWE2) in the ["Post Quantum"](https://cryptohack.org/challenges/post-quantum/) section.

Also use the references for the books mentioned for Task 2 if you like reading.

### The Interview
During the interview, we will review your progress - We will look at your CryptoHack account profile to see which challenges you have completed. Be ready to walk us through your solution for one of the
challenges you solved (or one you got stuck on).

### Evaluation Rubric

We will grade your submission based on the following criteria:

1. Practical Skill [70%] - Progress on the CryptoHack Lattice course. We value the difficulty of challenges solved over just the quantity.
2. Problem Solving [20%] -  Your approach to answering interview questions. Even if you don't know the exact answer, can you reason through it?
3. Communication [10%] - Clarity of thought. Can you explain complex mathematical concepts in simple terms?

## Task 2: Reading Project

### Textbook:

[Introduction to Modern Cryptography (2nd Edition)](https://eclass.uniwa.gr/modules/document/file.php/CSCYB105/Reading%20Material/%5BJonathan_Katz%2C_Yehuda_Lindell%5D_Introduction_to_Mo%282nd%29.pdf) by Jonathan Katz & Yehuda Lindell.

Optional additional reference: [Cryptobook](https://toc.cryptobook.us/book.pdf) by Daniel Boneh and Victor Shoup

### Objective:

1. Build a rigorous understanding of the "why" and "how" behind cryptographic security. This text moves beyond simple implementation to formal proofs and definitions.

### Required Reading Portions:

1. Chapters 1-4 (Boneh 2.1-2.3, 3.3, 3.4, 4.1-4.5, 12.2):

Foundations (Perfect Secrecy, Computational Security, Pseudorandomness, MACs).

2. Chapters 8-10 (Boneh 15.1-15.3, 16.1-16.5, 21.3, Appendix A):

Mathematical Hardness Assumptions (Number Theory, Factoring/DLP Algorithms, Key Exchange).

3. Section 11.5 (Boneh 12.3, 12.8, 16.4):

RSA Encryption (Plain RSA, Padded RSA, and Attacks).  

### Milestone Checkpoints

Use these questions to self-assess your understanding as you progress through the reading. You do not need to submit written answers, but you should be able to explain these concepts clearly during the interview.

1. Foundations (Chapters 1-4)

- Why is the One-Time Pad (OTP) considered "perfectly secret," and why is it impractical for most real-world uses?
- What is the difference between Perfect Secrecy and Computational Security? Why do we need the latter?
- Explain Kerckhoffs' Principle. Why is "security by obscurity" dangerous?
- Why is encryption alone insufficient for message integrity? How does a Message Authentication Code (MAC) fix this?

2. The Math & Algorithms (Chapters 8-10)
- What is the difference between the Factoring Assumption and the RSA Assumption? Which is stronger?
- Explain the Diffie-Hellman Key Exchange protocol. What specific problem allows two parties to generate a shared secret over an insecure channel?
- How do algorithms like Pollard's rho or the Quadratic Sieve improve upon trial division for factoring? Why does this matter for choosing key sizes?

3. RSA Specifics (Section 11.5)
- Why is "Textbook RSA" (deterministic RSA) insecure? Describe a simple attack against it.
- What is the role of padding (e.g., PKCS #1 v1.5) in making RSA secure?


### Evaluation Rubric

We will grade your submission based on the following criteria:


1. Theoretical Understanding [40%] - Ability to explain why a scheme is secure or insecure based on the reading. Can you define security properties (e.g., IND-CPA) rather than just describing the algorithm?
2. Practical Skill [30%] - Implementing attacks as you follow the book
3. Problem Solving [20%] -  Your approach to answering interview questions. Even if you don't know the exact answer, can you reason through it using the first principles you learned in the textbook?
4. Communication [10%] - Clarity of thought. Can you explain complex mathematical concepts in simple terms?

### The Interview
During the interview, we will ask conceptual questions derived from the Katz & Lindell chapters listed above. Be prepared to discuss the definitions and security proofs found in the text.
