# 🛡️ USB Device Security Auditor & Forensics Triage Tool

A lightweight, portable administrative tool designed for Windows environments to perform rapid security posture assessments, baseline compliance auditing, and incident response triage directly from a USB drive.

---

## 🚀 Key Features

- **Automated Security Baseline Scoring (0 - 100):**
  - Windows Defender status & signature definitions freshness.
  - Firewall profile verification.
  - BitLocker volume encryption status.
  - Legacy protocols check (SMBv1, LLMNR poisoning risk).
  - Exposure checks (Remote Desktop, Sensitive listening ports).
  - System hardening validation (UAC, Secure Boot, Guest Account).

- **DFIR & Forensics Triage:**
  - Historical USB device connection logs (Registry parsing).
  - Active local DNS cache dump.
  - Hosts file integrity and custom modifications check.
  - Suspicious Scheduled Tasks running outside system paths.
  - Persistence mechanisms (Clean startup programs inspection).

- **Network & Hardware Reconnaissance:**
  - Isolation of active primary IP, Gateway, and MAC address.
  - Connected Wi-Fi SSID identification.
  - Hardware specifications (CPU, RAM, Storage free space, Uptime).

- **Multi-Language Interactive Reports:**
  - Dual output: Structured **JSON** for programmatic analysis + Interactive **HTML** report.
  - Real-time search/filtering across all triage tables.
  - Dynamic **English / Arabic (RTL)** language toggle.
  - Print-ready CSS for direct PDF export.

---

## 🛠️ Built With

- **PowerShell 5.1+**
- **WMI / CIM Interfaces**
- **PS2EXE Compiler** (for portable standalone `.exe` execution)
- **HTML5 / CSS3 / Vanilla JavaScript**

---

## 💻 Usage

1. Copy `UsbAuditor.exe` to a USB flash drive.
2. Plug the USB into the target Windows workstation.
3. Run the executable as **Administrator**.
4. The tool will display a real-time summary in the console and automatically generate timestamped `.html` and `.json` audit reports in the same directory.
