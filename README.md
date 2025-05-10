# Mezel Honeypot

**A deceptive TCP sentinel engineered for reconnaissance, misdirection, and automated threat elevation.**

---

## Overview

**Mezel** is a lightweight, tactical honeypot designed for modern network environments where stealth, precision, and intelligence collection take priority over imitation.

Rather than simulating full services like SSH or HTTP, Mezel operates like a **tripwire wrapped in a black box**—detecting, fingerprinting, and reporting intrusions without revealing its hand.

---

## Why Mezel?

Most honeypots try to pretend.  
**Mezel doesn't. It listens, learns, and leaks attacker intel upstream.**

Mezel is built for operators who:

- Need immediate, high-signal alerts from inbound threats
- Prefer reaction and containment over engagement
- Want tight integration with real-world intel platforms (e.g. AbuseIPDB)
- Deploy honeypots **as tactical sensors**, not playgrounds

---

## Key Characteristics

- **Passive OS Fingerprinting**  
  Uses TCP behavior to infer attacker operating systems—*without sending a single packet back*.

- **Port Randomization & Rotation**  
  Avoids static signatures by listening on randomized ports each session.

- **Entropy Profiling**  
  Analyzes inbound payload structure—distinguishes scanners from toolkits, scripts from shells.

- **Threshold-Based Escalation**  
  Built-in emergency logic: when enough hits are detected, Mezel doesn't just log—it **adapts**.

- **External Intelligence Reporting**  
  Automatically reports verified hits to AbuseIPDB and can integrate with other feeds.

---

## Analogy for the Non-Technical

> **Imagine your network is a locked building.**  
>  
> **Mezel is not the guard at the front door.**  
> It’s the **fake electrical panel** in a utility closet. When a thief jimmies it open thinking it's vulnerable,  
> Mezel silently snaps a photo, triggers a silent alarm, and relays it to every nearby police unit—  
> **before the thief even knows he tripped a wire.**

---

## Use Cases

- **Private threat intelligence collection**
- **Edge deception systems** in corporate or personal networks
- **SOC/IR team augmentation**
- **Cyber observability nodes** in dark zones or DMZs

---

## How It's Different

| Feature                     | Mezel                   | Cowrie         | Glastopf       | T-Pot              |
|----------------------------|-------------------------|----------------|----------------|--------------------|
| Full protocol emulation    | No                      | SSH/Telnet     | HTTP           | Mixed              |
| Passive TCP fingerprinting | Yes                     | No             | No             | Partial            |
| Entropy scoring            | Yes                     | No             | No             | No                 |
| Auto escalation            | Yes (MAC/IP block, etc) | No             | No             | Varies             |
| External reporting         | Yes (AbuseIPDB, etc)    | Manual         | Manual         | Optional           |
| Setup complexity           | Low                     | Medium         | Low            | High (multi-service)|

---

## Status

- Currently in **field testing**
- Stable on Raspberry Pi and Linux servers
- Actively being refined with operational feedback

---

## License

Private / Restricted Use  
(Ask before deployment in shared or academic environments)

---

## Contributing

This project does not accept open pull requests yet, but feedback and usage insights are welcomed.

---

## Contact

For inquiries or controlled access, contact the project maintainer via this GitHub profile or encrypted channel.