# Suricata Threat Detection Rules

A curated list of custom Suricata rules to detect advanced network threats, CVEs, malware behavior, and unusual traffic patterns.
This repo serves to demonstrate threat detection capabilities and best practices when creating IDS/IPS rules.

---

## 📂 Repository Structure

rules/ # Core Suricata rules
├── cve/ # Rules for specific CVEs
├── malware/ # Malware-specific signatures (ransomware, trojans, etc.)
├── exploits/ # Exploit techniques not tied to CVEs (RCE, LFI, etc.)
├── traffic/ # Suspicious or anomalous traffic patterns (JA3, DNS, etc.)
└── custom/ # Experimental and PoC rules