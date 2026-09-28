<div align="center">

# 🔓 Password Cracking — Week 3

**Recovering a password from an encrypted PDF using John the Ripper and Networkwalks' online tools**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/John%20the%20Ripper-404040?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Johnny%20GUI-404040?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Password%20Cracking-C00000?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Hash%20Cracking-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
</p>

---

## 📌 Project Overview

This project documents **Week 3** of the Networkwalks Cybersecurity Internship: **password cracking**.

The goal was to recover the password of a deliberately locked/encrypted PDF file (`My Locked PDF1.pdf`) using two different approaches:

1. **John the Ripper (JTR) + Johnny GUI** — an industry-standard offline password cracking tool.
2. **Networkwalks' online Hash Calculator & Password Cracker** — free browser-based tools requiring no installation.

Comparing both approaches demonstrates how password/hash cracking works end-to-end: extracting a hash from a protected file, then running that hash through a cracking tool until a matching password is found.

---

## 🛡️ Authorization & Scope

This exercise was performed against a file (`My Locked PDF1.pdf`) provided specifically for this lab by Networkwalks, encrypted for training purposes only. No third-party or production systems/files were targeted.

⚠️ **Important:** Password cracking must only be performed on files/systems you own or have explicit written permission to test. Cracking passwords on files you do not own or lack authorization for is illegal in most jurisdictions.

---

## 🎯 Modules Covered

| Module | Topic | Tools Used |
|---|---|---|
| **W3-PM1** | Password Cracking with JTR | John the Ripper, Johnny GUI, onlinehashcrack.com (PDF hash extractor) |
| **W3-PM2** | Password Cracking with Networkwalks Tools | Networkwalks Hash Calculator, Networkwalks Password Cracker |

---

# 🪜 Module W3-PM1 — Password Cracking with JTR

**Target file:** `My Locked PDF1.pdf` (encrypted training PDF)

## Task
Crack the password of the attached PDF file using JTR John and JTR Johnny on a Windows PC.

## Step 1. Install John the Ripper & Johnny GUI

*(steps and screenshots to be added)*

## Step 2. Extract the PDF's Hash

The hash was extracted using [onlinehashcrack.com's PDF hash extractor](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php), then saved into a text file (`hash1.txt`) in the format `$pdf$...`.

*(steps and screenshots to be added)*

## Step 3. Crack the Hash with Johnny

The `hash1.txt` file was loaded into Johnny via "Open password file", and "Start new attack" was clicked to begin cracking.

*(steps and screenshots to be added)*

## Step 4. Open the PDF

*(steps and screenshots to be added)*

**Recovered password:** `[to be filled in]`

---

# 🪜 Module W3-PM2 — Password Cracking with Networkwalks Tools

**Target file:** `My Locked PDF1.pdf` (same file as W3-PM1)

## Task
Crack the password of the same locked PDF using the Networkwalks Hash Calculator and Password Cracker (browser-based, no installation required).

## Step 1. Extract the Hash — Networkwalks Hash Calculator

The PDF was uploaded to the [Networkwalks Hash Calculator](https://networkwalks.com/hash-calculator/), which returned a hash value starting with `$pdf$...`.

*(steps and screenshots to be added)*

## Step 2. Crack the Hash — Networkwalks Password Cracker

The hash was pasted into the [Networkwalks Password Cracker](https://networkwalks.com/password-cracker/) and the attack was started.

*(steps and screenshots to be added)*

## Step 3. Open the PDF

*(steps and screenshots to be added)*

**Recovered password:** `[to be filled in]`

---

### 📊 Comparison — JTR vs Networkwalks Tools

| Aspect | John the Ripper (JTR) | Networkwalks Tools |
|---|---|---|
| Installation required | Yes (JTR + Johnny GUI) | No (browser-based) |
| Platform | Windows / Linux / Mac | Any device with a browser |
| Hash extraction | Third-party tool (onlinehashcrack.com) | Built-in (Hash Calculator) |
| Time to crack | *(to be filled in)* | *(to be filled in)* |
| Ease of use for beginners | Moderate (GUI helps, but more setup) | Very easy (no setup) |

---

# 🐞 Problems Encountered & Solutions

*(to be filled in as tasks are completed)*

---

# 💡 What I Learned

- The difference between **encryption** (two-way, reversible with the correct key) and **hashing** (one-way, used to verify rather than reveal — though weak/short passwords can still be recovered by trying candidates against the hash).
- How a password-protected file's hash can be extracted and then attacked offline, independent of the original application (e.g. a PDF reader).
- Why password length and complexity matter: simple passwords can be cracked in minutes, while long, mixed-character passwords can take years.
- The practical trade-offs between a dedicated offline tool (JTR) and a quick browser-based tool (Networkwalks' tools) for the same task.

---

# 🔐 Security & Ethical Use

This repository is intended strictly for education and research purposes, as part of the Networkwalks Cybersecurity Internship. The target file was provided specifically for this training exercise. Do not use these tools or techniques against any file or system without explicit ownership or written permission.

---

# 🔗 Tools & Resources

- **John the Ripper:** [https://www.openwall.com/john/](https://www.openwall.com/john/)
- **Johnny GUI:** [https://openwall.info/wiki/john/johnny](https://openwall.info/wiki/john/johnny)
- **PDF Hash Extractor:** [https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php)
- **Networkwalks Hash Calculator:** [https://networkwalks.com/hash-calculator/](https://networkwalks.com/hash-calculator/)
- **Networkwalks Password Cracker:** [https://networkwalks.com/password-cracker/](https://networkwalks.com/password-cracker/)

---

# 👤 Author

**Boahene Prince**
Cybersecurity Intern, Batch B083B — Networkwalks

LinkedIn: [https://www.linkedin.com/in/boahene-prince-603b08372/](https://www.linkedin.com/in/boahene-prince-603b08372/)

---

## 📌 Project Information

**Program Name:** Cybersecurity at Networkwalks | **Week:** 03 | **Project:** Password Cracking (JTR + Networkwalks Tools) | **Repository:** GitHub
