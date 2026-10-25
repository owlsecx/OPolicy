# 🦉 OPolicy

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OPass-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OPolicy** — Password Policy Auditor & Advisor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OPolicy is a password-policy auditor and hardening advisor. It builds, parses and compares password policies from formats such as JSON, PAM, Windows GPO/secedit, AWS IAM and Keycloak, and evaluates them against standards including NIST SP 800-63B, CIS and PCI-DSS. It performs no cracking and uses no online APIs.

---

## ✨ Features

- Interactive policy builder covering length, complexity, lockout, MFA and breach screening
- Policy parser for JSON, PAM, Windows GPO/secedit, AWS IAM and Keycloak formats
- Standards engine (NIST, CIS, PCI-DSS, ISO 27001, Microsoft, Google) with per-control results
- Plaintext password-list auditor with entropy, pattern and compliance analysis
- Offline breach-pattern detection and policy-to-policy comparison
- Remediation generator (pam_pwquality, faillock, GPO, FreeIPA, Keycloak, Okta, AWS IAM) with TXT/CSV/JSON export

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OPolicy -p policy.json -s nist,cis
./OPolicy --audit-list passwords.txt --company acme
./OPolicy -p policyA.json --compare policyB.json
./OPolicy --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
