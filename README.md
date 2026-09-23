# Cybersecurity Internship | Week 3: Password Cracking & Hash Analysis Project

A comprehensive, hands-on penetration testing lab report focusing on cryptographic hash extraction, offline password auditing, and brute-force/dictionary attacks utilizing **John the Ripper (CLI)**, **Johnny GUI**, and web-based utilities.

---

## 📌 Executive Summary & Project Overview
During Week 3 of the cybersecurity internship program, practical assessments were performed to evaluate the resilience of cryptographic hashes extracted from protected assets (such as locked PDF documents). Using both offline engine wrappers like **John the Ripper** and **Johnny GUI**, alongside online hash calculators and dictionary crackers, hashes were successfully audited to demonstrate the inherent vulnerabilities associated with weak, predictable passwords and legacy file encryption standards.

---

## 🛠️ Technical Stack & Tools Utilized
* **Primary Environment:** Windows Operating System
* **Offline Cracking Suite:** John the Ripper (JTR) - Jumbo Edition (`john.exe`)
* **Graphical Interface (GUI):** Johnny Password Cracker Frontend
* **Web-Based Utilities:** Networkwalks Hash Calculator & Online Password Cracker
* **Target Artifacts:** Password-protected / encrypted PDF files
* **Outcome Status:** 100% Attack Success Rate (Credentials & Flags Successfully Recovered)

---

## 🚀 Detailed Step-by-Step Lab Implementation

### Step 1: Initial Cryptographic Hash Extraction from Target Files
* **Objective:** Extract crackable cryptographic hash structures from a password-protected PDF document.
* **Execution:** Utilizing an authorized web-based PDF Hash Extractor utility, the target encrypted PDF file was processed to extract standard hash string configurations compatible with `pdf2john` and hash-cracking frameworks.

<img width="1920" height="1080" alt="Online PDF Hash Extraction" src="week3 8 _2.png" />

---

### Step 2: Hash Preservation and Text File Preparation
* **Objective:** Structure and format the extracted hash for batch processing.
* **Execution:** The raw hash string output (`$pdf$4*4*128*...`) was copied, organized, and saved into a plain text file named `hash1.txt` using a text editor (Notepad), establishing a clean input source for subsequent offline auditing tools.

<img width="1920" height="1080" alt="Hash Preserved in Notepad" src="week3 9_2.png" />

---

### Step 3: Johnny GUI Application Launch & Workspace Initialization
* **Objective:** Initialize the graphical user interface wrapper for John the Ripper.
* **Execution:** Launched the Johnny GUI application on the local Windows environment to prepare a centralized workspace for managing password sessions, loading target hashes, and orchestrating attacks.

<img width="1920" height="1080" alt="Johnny GUI Initial State" src="week3   6 .png" />

---

### Step 4: Engine Path Configuration & Binary Linkage
* **Objective:** Link the graphical frontend to the core John the Ripper engine executable.
* **Execution:** Navigated to the application Settings menu, pointed the "John the Ripper executable" field to the core binary file (`john.exe` located within the JTR jumbo distribution directory), and successfully verified engine detection (`Detected John the Ripper 1.9.0-jumbo-1 OMP`).

<img width="1920" height="1080" alt="Johnny GUI Path Configuration" src="week3 7.png" />

---

### Step 5: Successful Offline Password Recovery & Execution
* **Objective:** Execute dictionary and brute-force routines against the loaded hash file.
* **Execution:** After importing the hash file into Johnny GUI, the attack sequence was initiated. The tool systematically processed the wordlist entries, successfully recovering the target password (`password1`) with a 100% completion rate (1/1 cracked, 0 left).

<img width="1920" height="1080" alt="Successful Crack in Johnny GUI" src="week3 11_2.png" />

---

### Step 6: Alternative Methodology - Networkwalks Hash Calculator
* **Objective:** Explore web-based text hashing and PDF hash parsing utilities.
* **Execution:** Accessed the Networkwalks Hash Calculator tool to examine alternative techniques for generating checksums (MD5, SHA variants) and extracting crackable hashes locally within the browser context.

<img width="1920" height="1080" alt="Networkwalks PDF Hash Extraction" src="week3 2.png" />

---

### Step 7: Online Password Cracker Configuration
* **Objective:** Set up a controlled web-based dictionary attack environment.
* **Execution:** Pasted the extracted PDF hash into the Networkwalks Online Password Cracker utility and configured the execution parameters to leverage a pre-loaded built-in wordlist containing standard common passwords.

<img width="1920" height="1080" alt="Online Cracker Configuration" src="week3 3.png" />

---

### Step 8: Online Attack Validation and Verification
* **Objective:** Cross-verify offline cracking outcomes using a web-based interface.
* **Execution:** The online password cracking engine rapidly iterated through the dictionary words, successfully matching the hash and confirming the recovered credential (`password1`), validating the consistency of both auditing approaches.

<img width="1920" height="1080" alt="Online Crack Success" src="week3  4.png" />

---

### Step 9: Final Milestone Achievement & Flag Capture
* **Objective:** Conclude the lab module and secure confirmation of successful task execution.
* **Execution:** Completed all required assessment phases, resulting in the successful capture of the internship project flag (`nw{networkwalks_persistence_jtr_270521}`), verifying comprehensive proficiency in credential auditing.

<img width="1920" height="1080" alt="Flag Captured" src="week3  5.png" />

---

## ⚠️ Risk Analysis & Business Impact
* **Vulnerability to Dictionary Attacks:** The rapid recovery of human-readable credentials (such as `password1`) highlights the catastrophic risk of utilizing common passphrases for protecting confidential documentation.
* **Legacy Algorithm Constraints:** Older file encryption formats often implement cryptographic derivation functions that prioritize speed over security, making them heavily susceptible to multi-core CPU and GPU-accelerated cracking tools.

---

## 🛡️ Remediation & Security Recommendations
1. **Enforce Robust Password Complexities:** Mandate the use of long, highly complex passphrases incorporating a diverse mix of uppercase letters, lowercase letters, numeric digits, and special symbols.
2. **Upgrade Encryption Standards:** Transition away from legacy, easily crackable file formats and adopt modern, enterprise-grade encryption mechanisms (such as AES-256).
3. **Proactive Credential Auditing:** Regularly perform authorized internal password audits to identify weak or default credentials before external malicious entities can exploit them.

---
*Authorized Cybersecurity Portfolio Project — Developed as part of the Internship Training Curriculum.*
