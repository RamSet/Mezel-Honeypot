# Mezel Honeypot
**An active threat intelligence engine for deception, detection, and dynamic response.**

---

## Overview

**Mezel** isn’t just a honeypot — it’s an evolving **threat operations platform**.  
Built from the ground up through hundreds of iterations and field-tested edge cases, Mezel detects, classifies, and responds to hostile network traffic with surgical precision.

Designed for operators, security teams, and research environments that demand more than logs — Mezel delivers **actionable intelligence** and the ability to respond in real time.

---

## Why Mezel?

Other honeypots try to fool attackers.  
**Mezel doesn’t play games — it collects evidence and pulls triggers.**

It’s built for environments where:
- **Speed and signal matter more than simulation**
- **Deception is a tactic, not a gimmick**
- **Threat data must flow upward, outward, and into enforcement layers**

---

## Current Capabilities

### Modular Intelligence Stack
Mezel is composed of decoupled, resilient modules:
- **AbuseIPDB Reporter** (offline-aware, cached, rate-limited)
- **YARA Payload Scanner**
- **ZyWALL + Fortinet Firewall Integrators**
- **Passive Fingerprinter**
- **Entropy Analyzer**
- **Geo Dashboard Renderer**
- **Pushover Notification Engine**

Each module is deployable, restartable, and independently testable.

---

### Firewall-Integrated Deception
- **ZyWALL integration**: MAC-to-IP mapping, threat containment
- **Fortinet roadmap**: Real-time API interaction to enable address bans, tag sessions, or trigger FortiAnalyzer events
- This turns Mezel into **an automated enforcement node**, not just a sensor.

---

### Live Payload Triage with YARA
Inbound data is scanned against YARA signatures to detect:
- Malware families
- Botnet payloads
- Encoded reverse shells
- Exploit kit markers

This lets you classify attacks immediately, not retroactively.

---

### Full Internet-Aware Abuse Reporting
- Sends structured reports to AbuseIPDB
- Includes attacker IP, port, payload, entropy, matched YARA rules, and context
- Smart queuing: delays submission when internet drops
- Smart notifications: resumes when back online, notifies of backlogs, clears, and first success

---

### Dashboard Telemetry
- Map visualizations of incoming hits
- Payload previews with syntax highlighting
- Live entropy and YARA-tagged feed
- Optional auto-refresh for SOC displays

---

### Real-Time Alerting
Pushover notifications for:
- First hit
- Abuse submission success/failure
- Queue overload
- Internet loss/recovery
- Daemon shutdowns

---

### Built to Operate Unattended
- Can run headless on Raspberry Pi
- Works on ARM or x86
- Systemd-managed, service-ready
- Survives power loss, network failure, or abuse floods

---

## Analogy for the Non-Technical

> Imagine your network is a house.  
> You don’t put Mezel at the front door — you put it **inside the wall, behind a fake outlet**.  
>
> When a burglar pokes it thinking it’s a weak point, Mezel:
> - **Fingerprints their tools**
> - **Captures a copy of their lockpick**
> - **Scans the fingerprint against a criminal database**
> - **Notifies security instantly**
> - And if you’re connected to smart locks or drones,  
>   **it’ll lock them in the hallway before they know what hit them.**

---

## Use Cases

- **SOHO + Enterprise Deception Layer**
- **Threat Research Collection**
- **Automated Abuse Reporter**
- **Firewall-Orchestrated Containment**
- **Live Attack Dashboard Feeds**

---

## Comparison Matrix

| Feature                     | Mezel                   | Cowrie         | Glastopf       | T-Pot              |
|----------------------------|-------------------------|----------------|----------------|--------------------|
| Full protocol emulation    | No                      | SSH/Telnet     | HTTP           | Mixed              |
| Passive TCP fingerprinting | Yes                     | No             | No             | Partial            |
| Entropy scoring            | Yes                     | No             | No             | No                 |
| YARA scanning              | Yes                     | No             | No             | No                 |
| Abuse reporting            | Yes (robust)            | Manual         | Manual         | Optional           |
| Offline awareness          | Yes                     | No             | No             | No                 |
| Fortinet/ZyWALL firewall   | Yes (live & roadmap)    | No             | No             | No                 |
| Dashboard telemetry        | Yes                     | No             | No             | Varies             |
| Setup complexity           | Moderate                | Medium         | Low            | High               |

---

## Development Status

- Stable and field-hardened
- Modularized into deployable components
- Actively expanding Fortinet support
- Ready for testbeds, darknets, SOCs, or live edge deployments

---

## License

Private / Controlled Use  
(Request access for threat labs, security orgs, or academic research)

---

## Contact

Reach out via GitHub or secure messaging for deployment requests, contributions, or integration discussions.
