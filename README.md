# 🛡️ Cybersecurity Internship
## Week 3: Password Cracking & Hash Analysis Project

A comprehensive, hands-on penetration testing lab report focusing on cryptographic hash extraction, offline password auditing, and brute-force/dictionary attacks utilizing **John the Ripper (CLI)**, **Johnny GUI**, and web-based utilities.

---

## 📌 Executive Summary & Project Overview

During Week 3 of the cybersecurity internship program, practical assessments were performed to evaluate the resilience of cryptographic hashes and encrypted files (such as password-protected PDF documents). 

In this project, we successfully completed two primary tasks: first, using the **Networkwalks web-based calculator** for hash generation, file conversion, and online dictionary attacks; and second, performing offline cryptographic hash extraction and auditing using **John the Ripper (JTR)** and **Johnny GUI** to uncover weak, predictable passwords and recover hidden flags.

---

## 🛠️ Technical Stack & Tools Utilized

* **Primary Environment:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Windows Operating System
* **Offline Cracking Suite:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;John the Ripper (JTR) - Jumbo Edition (`john.exe`)
* **Graphical Interface (GUI):**&nbsp;&nbsp;&nbsp;&nbsp;Johnny Password Cracker Frontend
* **Web-Based Utilities:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Networkwalks Hash Calculator & Online Password Cracker
* **Target Artifacts:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Password-protected / encrypted PDF files
* **Outcome Status:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;100% Attack Success Rate (Credentials & Flags Successfully Recovered)

## 🚀 Part 1: Password Cracking Process

### Step 1.1: Networkwalks Hash Calculator Interface
* **Description:** Access kiya gaya Networkwalks Hash Calculator home page jahan text, file, aur PDF conversion ke options available hain.
* **Screenshot:**
  ![Hash Calculator Home](week%203%201.png)

### Step 1.2: PDF File Upload & Hash Extraction
* **Description:** Locked PDF file (`My-Locked-PDF2.pdf`) ko upload kar ke uska crackable cryptographic hash format successfully extract kiya gaya.
* **Screenshot:**
  ![PDF Hash Calculation](week3%202.png)

### Step 1.3: Dictionary Attack Configuration
* **Description:** Extracted hash ko Networkwalks Password Cracker tool mein paste kiya gaya aur built-in wordlist select ki gayi.
* **Screenshot:**
  ![Online Password Cracker](week3%203.png)

### Step 1.4: Successful Password Cracking
* **Description:** Dictionary attack successfully run hone ke baad password (`password1`) recover ho gaya.
* **Screenshot:**
  ![Online Attack Success](week3%204.png)

### Step 1.5: Final Flag Capture
* **Description:** PDF unlock hone ke baad final project flag successfully capture kar liya gaya.
* **Screenshot:**
  ![Final Flag Capture](Screenshot%202026-09-24%20134552.png)
