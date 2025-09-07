# Suricata Threat Detection Rules

A curated list of custom Suricata rules to detect advanced network threats, CVEs, malware behavior, and unusual traffic patterns.
This repo serves to demonstrate threat detection capabilities and best practices when creating IDS/IPS rules.

---

## 📂 Repository Structure

```text
rules/              # Core Suricata rules
├── cve/            # Rules for specific CVEs
├── malware/        # Malware-specific signatures (ransomware, trojans, etc.)
├── exploits/       # Exploit techniques not tied to CVEs (RCE, LFI, etc.)
├── traffic/        # Suspicious or anomalous traffic patterns (JA3, DNS, etc.)
└── custom/         # Experimental and PoC rules
```

## 🔢 SID Allocation Plan

To avoid collisions and preserve rules traceable, the following SID ranges are used by this repository:

```text
| Range              | Category            |
|--------------------|---------------------|
| 1000000–1099999    | CVE rules           |
| 1100000–1199999    | Malware rules       |
| 1200000–1299999    | Exploit techniques  |
| 1300000–1399999    | Traffic anomalies   |
| 1400000–1499999    | Custom/PoC rules    |