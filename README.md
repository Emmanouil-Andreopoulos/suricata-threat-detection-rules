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
| 1000000–1000999    | CVE rules           |
| 1001000–1001999    | Malware rules       |
| 1002000–1002999    | Exploit techniques  |
| 1003000–1003999    | Traffic anomalies   |
| 1009000–1009999    | Custom/PoC rules    |
```