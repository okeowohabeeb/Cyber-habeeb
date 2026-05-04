# 🕵️‍♂️ Offensive Security: FakeBank – Hidden Directory Discovery

**Platform:** TryHackMe  
**Room:** PreSecurity – Offensive Security Intro  
**Focus:** Web Enumeration / Directory Brute‑forcing  
**Date:** [2026-05-04]

---

## 🎯 Objective
*Find a hidden page on the FakeBank website and exploit it to transfer money without authorisation.*

---

## 🛠️ Tools Used
- **Gobuster** – a directory/file brute‑forcing,nmap. 

---
___
## 🔍 Finding
A hidden directory `/bank-transfer` that allowed unauthorised money transfers.” `BANK-HACKED` message 

## 🌍 Real‑world Significance (Offensive Perspective)
 *Hidden directories are treasure troves for attackers. Tools like Gobuster make discovery trivial. Once found, broken access controls (IDOR) let attackers act as other users – stealing funds, altering records, or escalating privileges.*]

## ✅ Lessons Learned

- **Enumerate everything** – Attackers never assume a hidden page is safe.
- **Test authorisation thoroughly** – Don't trust that a hidden URL means hidden permissions.
- **Think like an attacker** – Use the same tools (Gobuster, Burp, Nmap) to discover my own weaknesses.
- **Document findings clearly** – A good report turns a hack into a fix.

> *These lessons apply directly to penetration testing, red teaming, and bug bounty hunting.*
## ⌨️ Commands Executed  

```bash
gobuster dir -u http://fakebank.thm -w /path/to/wordlist.txt
