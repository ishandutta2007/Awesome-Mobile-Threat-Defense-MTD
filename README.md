# Awesome-Mobile-Threat-Defense-MTD

## Top Mobile Threat Defense (MTD) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on On-Device Threat Detection, Privacy-Preserving Security & Self-Hosted Mobile Hardening*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Mobile Threat Defense (MTD)**. These tools enable organizations and individuals to protect mobile devices—iOS and Android—against device compromise, malicious apps, network attacks, and phishing, while respecting user privacy and data ownership.



**Examples** include CrowdStrike Falcon Mobile Security, Zimperium, Lookout Mobile Endpoint Security, Wandera (Jamf), Microsoft Defender for Mobile, Harmony Mobile (Check Point), Pradeo, Sophos Mobile, Symantec Endpoint Protection Mobile, and Trend Micro Mobile Security (the category leaders).



**Open-source emphasis**: Mobile Threat Defense is a domain where open-source tooling is **severely limited and fundamentally consumer-scoped, not enterprise-grade**. The only OSI-approved entry in the MTD category is **Hypatia**—an Android-only, on-device malware scanner using ClamAV signatures, explicitly positioned as a consumer/privacy-focused tool rather than an enterprise MTD platform . **ShieldApp** offers a surprisingly comprehensive Android security suite (antivirus with YARA, phishing detection, Tor VPN, breach monitoring, and 50+ tools) but it is a consumer app with no central management console . **HubSecurityArtificialIntelligence** is an early-stage research project claiming a Mobile Threat Defense module for SMS phishing detection, but it is a personal project, not a production platform . The critical caveat: **no open-source project matches the enterprise MTD capabilities** of Zimperium (on-device ML detection without cloud dependency) , Lookout (150M+ device dataset, UEM integration, EDR response) , or Check Point Harmony (behavioral risk engine, gateway, and dashboard) . Enterprise MTD requires MDM/UEM integration, central policy enforcement, and threat forensics—none of which open-source currently provides.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon Mobile Security](https://www.crowdstrike.com/)**  

  Mobile threat defense integrated into the Falcon platform; protects iOS and Android devices against app, network, phishing, and device threats.



- **[Zimperium](https://www.zimperium.com/)**  

  Enterprise MTD with **on-device, machine-learning-powered detection** that works even without network connectivity; protects against device, network, app, and phishing attacks without compromising employee privacy (cannot read texts, emails, browsing history, or files) . Integrates with leading MDM/EMM/UEM, SIEM, and SOAR platforms for risk-based policy enforcement and forensics .



- **[Lookout Mobile Endpoint Security](https://www.lookout.com/)**  

  Cloud-based MTD with a lightweight endpoint app and near-real-time visibility into mobile risk; integrates with leading UEM (VMware Workspace ONE, Ivanti, IBM MaaS360, Samsung Knox) and SIEM systems via Mobile Risk API . Leverages a dataset from **150M+ devices and 50M+ apps**, with endpoint detection and response (quarantine + self-remediation instructions) .



- **[Wandera (Jamf)](https://www.jamf.com/)**  

  Mobile security and data usage management platform (acquired by Jamf); provides threat defense and policy enforcement for mobile fleets.



- **[Microsoft Defender for Mobile](https://learn.microsoft.com/defender-endpoint/mtd)**  

  MTD for Android and iOS integrated into Microsoft Defender for Endpoint; features **Web Protection** (phishing blocking, custom URL/domain indicators), **Malware Protection** (Android only, scans apps and non-APK files), **Jailbreak/Root Detection**, **Network Protection** (Wi-Fi threats, fake certificates), **Vulnerability Management**, and **Conditional Access** to block risky devices from corporate resources .



- **[Harmony Mobile (Check Point)](https://www.checkpoint.com/)**  

  Enterprise MTD with a **Behavioral Risk Engine**, Gateway, Management Dashboard, and Protect app for iOS/Android; performs advanced app analysis to detect known and unknown threats, prevents man-in-the-middle attacks on cellular/Wi-Fi, blocks phishing across all apps, and prevents infected devices from accessing corporate data .



- **[Pradeo](https://www.pradeo.com/)**  

  Mobile threat defense and app security platform; focuses on app behavior analysis and compliance.



- **[Sophos Mobile](https://www.sophos.com/)**  

  Mobile device management and security with MTD capabilities; integrates with Sophos endpoint protection.



- **[Symantec Endpoint Protection Mobile](https://www.broadcom.com/)**  

  Mobile threat defense within Broadcom's endpoint security portfolio (formerly Skycure); protects against network, device, and app threats.



- **[Trend Micro Mobile Security](https://www.trendmicro.com/)**  

  Mobile security with threat defense and device management for enterprise fleets.



## Open-Source GitHub Projects



### Android Security Suites (Consumer-Scoped)



- **[Hypatia](https://github.com/Divested-Mobile/Hypatia)**  

  The **only OSI-approved open-source MTD-adjacent entry** available (GPL-3.0) . An **Android-only on-device malware scanner** using **ClamAV signatures**; consumer/privacy-focused, with no central management, network protection, or phishing detection. DivestOS-adjacent project. **Best for privacy-conscious Android users** wanting local malware scanning—but it is **not an enterprise MTD** (no UEM integration, no policy enforcement, no forensics) .



- **[ShieldApp](https://github.com/beenuar/shieldapp-android)**  

  The **most feature-dense open-source Android security suite** (MIT, Kotlin/Compose) . Features: **antivirus engine** (signature + heuristic + YARA, 54,000+ signatures, 9 real-time feeds); **deepfake detection** (TensorFlow Lite/ML Kit); **scam call/SMS shield**; **Tor VPN** (all traffic routed through Tor with 24 exit countries); **dark web/breach monitoring** (HIBP k-anonymity); **network monitor**; **app auditor** (25 permission categories, 21 tracker SDKs); **phishing scanners** (email, SMS, QR); **Wi-Fi threat detection**; **secure notes vault**; and 50+ tools. **All on-device, no cloud, no API keys, no telemetry** . **Best for technically-savvy Android users** wanting maximum personal protection—but it is a **consumer app with no central management console**, not an enterprise MTD platform.



- **[Cybe](https://github.com/cyberlog69/Cybe-App)**  

  Cross-platform (Android/iOS) mobile security and privacy suite with **Wi-Fi threat shield** (ARP spoofing, SSL stripping, DNS hijacking detection), **antivirus** (SHA-256/YARA heuristics), **phishing URL checker**, **vulnerability audit** (root/emulator/patch staleness checks), **encrypted DNS (DoH)**, **LAN port scanner**, and **duress panic wipe** . **Best for individual users** wanting a broad security toolkit—but it is consumer-focused and not enterprise-managed.



### Research & Early-Stage Projects



- **[HubSecurityArtificialIntelligence](https://github.com/murdok1982/HubSecurityArtificialIntelligence)**  

  An early-stage **AI-driven defensive ecosystem** (FastAPI/PostgreSQL/Docker/Celery) that claims a **Mobile Threat Defense (MTD) module** for detecting SMS phishing and scam activity, alongside desktop EDR and threat intelligence feeds . **Critical caveat**: it is a personal research project shared on LinkedIn, not a production platform—no documentation, no enterprise features, and unverified claims. **Best for researchers** exploring AI-driven mobile threat detection patterns—but **not suitable for production or enterprise use**.



### Additional Strong Open-Source Options



- **MobARK** — Self-hosted **mobile application security testing** platform (Android APK/iOS IPA static analysis with Semgrep, Gitleaks, and AI agent) . **Not an MTD**—it is a pentesting/AppSec tool for analyzing apps you build or assess, not for protecting devices in the field.

- **catbyte-toolkit** — macOS/iOS binary analysis toolkit for security research (recon, vuln scanning, exploit dev) . **Not an MTD**—it is a research toolkit for reverse engineering, not device protection.



**Frameworks for building custom systems**: For **Android malware scanning**, Hypatia provides a privacy-focused local AV . For **comprehensive consumer Android protection**, ShieldApp offers the broadest feature set (antivirus, VPN, phishing, breach monitoring) . For **research into AI-driven mobile threat detection**, HubSecurityArtificialIntelligence demonstrates the pattern but is not production-ready . **No open-source project provides enterprise MTD**—the commercial platforms (Zimperium, Lookout, Microsoft Defender, Check Point Harmony) are required for MDM/UEM integration, central policy enforcement, threat forensics, and risk-based conditional access .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Mobile Threat Defense platforms handling device and user data must comply with applicable privacy regulations (GDPR, CCPA) and organizational security policies; **enterprise MTD must balance security visibility with employee privacy**—Zimperium explicitly cannot read texts, emails, browsing history, or files , and Lookout states it does not collect images, audio, video, texts, or personal information .

- **Open-source Mobile Threat Defense is severely limited**—the only OSI-approved entry (Hypatia) is a **consumer Android malware scanner**, not an enterprise MTD . ShieldApp and Cybe are comprehensive consumer suites but lack central management . **No open-source project matches the enterprise capabilities** of Zimperium (on-device ML detection, MDM/UEM integration) , Lookout (150M+ device dataset, SIEM integration) , or Microsoft Defender (Conditional Access, vulnerability management) . Organizations requiring enterprise MTD should evaluate commercial platforms.

- Verify license terms for commercial use; Hypatia uses GPL-3.0 , ShieldApp uses MIT , and Cybe is open-source (check repository).



---



**Made for security architects, mobile administrators, and organizations choosing their mobile threat defense stack.**  

Let's make mobile threat defense more open, but with clear eyes about the enterprise management and MDM integration gap that commercial platforms still fill.
