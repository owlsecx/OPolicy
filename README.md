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

Password policy auditor & compliance hardening advisor (NIST, CIS, PCI-DSS, PAM, GPO)

---

## ✨ Features

- Interactive policy builder — length, complexity, history, lockout, MFA, expiry, blocklist, breach screening, paste, hints, KBA; scored A+…F report
- Policy parser — JSON, key=value, free text, Windows secedit INF / `net accounts` / GPO, Linux PAM (pwquality, pam_unix, faillock, login.defs), AWS IAM JSON and Keycloak policy strings
- Standards engine — NIST SP 800-63B, CIS, PCI-DSS 4.0, ISO 27001, Microsoft, Google Workspace, AD defaults with per-control pass / fail / warn and coverage %
- Password-list auditor (plaintext only) — length histogram, charset mix, entropy, keyboard walks, dates, leetspeak, repeats, sequences, reused prefixes / suffixes, compliance % vs a policy
- Breach-pattern detector — offline pattern library (season+year, Name123!, qwerty, company+year, ...)
- Policy comparison — field diff and gap analysis
- Remediation generator — pam_pwquality, faillock, GPO registry / PowerShell, FreeIPA, Keycloak, Okta, AWS IAM password policy JSON
- Save report (TXT / CSV / JSON) with location chooser
- Full CLI mode (-p policy.json --standard all, ...)

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OPolicy
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
