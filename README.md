# Awesome Mobile Threat Defense (MTD) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of leading Mobile Threat Defense (MTD) platforms, mobile endpoint detection and response (EDR), and open-source mobile security frameworks.

Mobile Threat Defense (MTD) solutions protect iOS, iPadOS, Android, and ChromeOS devices from advanced mobile security risks spanning four primary attack vectors: **device vulnerabilities** (jailbreak/rooting, OS exploits, configuration drift), **network threats** (man-in-the-middle attacks, SSL stripping, malicious Wi-Fi, rogue cellular base stations), **application risks** (spyware, malware, aggressive trackers, leaky permissions), and **phishing & content threats** (SMS smishing, QR-code phishing, malicious URLs across messaging and email).

---

## Sector Overview & Market Dynamics

The global Mobile Threat Defense (MTD) market is estimated at approximately **$4.0 billion to $4.9 billion in 2025–2026**, expanding rapidly at a compound annual growth rate (CAGR) of **15% to 24%** driven by enterprise Bring-Your-Own-Device (BYOD) adoption, hybrid remote workforces, and the surge in AI-orchestrated mobile smishing and zero-day app vulnerabilities. The sector is **moderately concentrated**: established cybersecurity and infrastructure titans control roughly 60% of enterprise market share through tight integrations with Unified Endpoint Management (UEM/MDM) and XDR platforms, while specialized pure-play vendors and on-device behavioral ML engines command the remainder of high-assurance deployments.

---

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS & Enterprise MTD Platforms](#saas--enterprise-mtd-platforms)
- [Open-Source Mobile Security Projects](#open-source-mobile-security-projects)
- [Enterprise vs Open-Source Comparison](#enterprise-vs-open-source-comparison)
- [How to Contribute](#how-to-contribute)
- [License & Disclaimer](#license--disclaimer)

---

## SaaS & Enterprise MTD Platforms

The following enterprise platforms provide comprehensive Mobile Threat Defense (MTD) capabilities, including on-device real-time behavioral protection, MDM/UEM conditional access integration, fleet-wide risk dashboards, and automated incident remediation.

*Table is sorted descending by Company Size (Market Capitalization / Valuation / Revenue).*

| Platform | Company Size (Market Cap / Valuation / Revenue) | Starting Pricing (Specific Tier) | Free Tier / Trial Limit | Key MTD Capabilities & Target Fleet |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Defender for Mobile](https://learn.microsoft.com/defender-endpoint/mtd)** | ~$3.1T Market Cap (Microsoft) | $3.00 / user / month (Defender for Endpoint Plan 1 or Defender for Business) | 90-day free trial (Full enterprise feature evaluation via Microsoft 365 Admin Center) | Web protection, anti-phishing, jailbreak/root detection, network protection, vulnerability management, and Intune Conditional Access gating. |
| **[Symantec Endpoint Protection Mobile](https://www.broadcom.com/)** | ~$1.55T Market Cap (Broadcom) | $50.00 / device / year (~$4.17/mo, SEP Mobile 1-year standalone subscription list tier) | 30-day proof-of-concept trial via Broadcom Enterprise authorized reseller or direct sales | On-device network protection against Wi-Fi MITM, app analysis, vulnerability shielding, and enterprise SIEM/UEM bidirectional connectors. |
| **[CrowdStrike Falcon for Mobile](https://www.crowdstrike.com/)** | ~$260B Market Cap (~$5.4B ARR) | $59.99 / device / year (~$5.00/mo billed annually on Falcon Go) | 15-day free trial (Instant self-service onboarding, no credit card required, covers up to 100 endpoints) | Real-time behavioral EDR on iOS/Android, malicious app detection, phishing protection, and integration into the CrowdStrike Falcon XDR platform. |
| **[Harmony Mobile (Check Point)](https://www.checkpoint.com/)** | ~$15B Market Cap (~$2.6B Revenue) | $40.00 / device / year (~$3.33/mo per-device annual subscription tier) | 30-day free trial (Full enterprise Infinity Portal access with active mobile behavioral engine) | Behavioral risk engine, on-device network inspection, anti-phishing across all messaging apps, and conditional corporate access controls. |
| **[Trend Micro Mobile Security Enterprise](https://www.trendmicro.com/)** | ~$6.2B Market Cap (~$1.7B ARR) | $30.00 / device / year (~$2.50/mo commercial seat starting bracket) | 30-day enterprise evaluation / PoC trial (via Trend Micro Cloud One / Worry-Free Services console) | Application reputation service, web threat defense, ransomware protection, Wi-Fi auditing, and centralized enterprise fleet policies. |
| **[Wandera / Jamf for Mobile](https://www.jamf.com/)** | ~$1.74B Market Cap (~$600M Revenue) | $5.75 / device / month (billed annually, 25-device minimum on Jamf for Mobile) | 14-day to 30-day free trial (Cloud evaluation instance, no credit card required) | Mobile threat defense, zero-trust network access (ZTNA), content filtering, data policy enforcement, and native Apple/Android ecosystem optimization. |
| **[Sophos Mobile Advanced](https://www.sophos.com/)** | ~$1.0B Revenue (Thoma Bravo PE) | $46.80 / user / year (~$3.90/mo list tier for 1–9 users on Sophos Central Mobile Advanced) | 30-day free trial (Sophos Central cloud trial, unthrottled access across mobile security features) | Unified Endpoint Management (UEM) combined with Intercept X for Mobile, on-device deep learning malware scanner, and web filtering. |
| **[Lookout Mobile Endpoint Security](https://www.lookout.com/)** | ~$1.5B Private Valuation (~$135M ARR) | $50.00 / device / year (~$4.17/mo for Lookout MES Essentials bundle) | 30-day free trial (Enterprise fleet proof of concept, available directly or via AWS Marketplace) | Cloud-scale threat engine powered by 150M+ devices/50M+ apps, proactive smishing blocking, app vetting, and automated quarantine workflows. |
| **[Zimperium Mobile Threat Defense](https://www.zimperium.com/)** | $525M Acquisition Valuation (~$50M Revenue) | $48.00 / device / year (~$4.00/mo enterprise base bracket on AWS Marketplace / Resellers) | 30-day free trial (Enterprise PoC tenant with z9 on-device machine-learning engine deployment) | Patented on-device machine learning (z9 engine) operating without cloud roundtrips, zero employee privacy invasion, and MDM/SIEM/SOAR automation. |
| **[Pradeo Mobile Threat Defense](https://www.pradeo.com/)** | ~$5M–$10M Revenue (~$1.4M Funding) | €16.00 / device / year (~€1.33/mo standard baseline license tier) | 30-day free trial (Complete access to Pradeo Security SaaS console and mobile test agents) | Specialized 360-degree mobile app behavior analysis, network protection, OS exploit shielding, and GDPR/privacy-first compliance profiling. |

---

## Open-Source Mobile Security Projects

Open-source tooling in mobile security excels at forensic analysis, static/dynamic APK/IPA security auditing, network telemetry inspection, and local consumer malware scanning. 

*Table is sorted descending by GitHub Star Count.*

| Project | Stars | Focus Area | Platform | Description & Architecture |
| :--- | :--- | :--- | :--- | :--- |
| **[MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF)** | [![GitHub stars](https://img.shields.io/github/stars/MobSF/Mobile-Security-Framework-MobSF?style=social&color=white)](https://github.com/MobSF/Mobile-Security-Framework-MobSF/stargazers) | Automated AppSec & Malware Analysis | Android / iOS / Windows | Automated, all-in-one mobile application pen-testing, malware analysis, and security assessment framework performing static and dynamic binary analysis. |
| **[MVT (Mobile Verification Toolkit)](https://github.com/mvt-project/mvt)** | [![GitHub stars](https://img.shields.io/github/stars/mvt-project/mvt?style=social&color=white)](https://github.com/mvt-project/mvt/stargazers) | Digital Forensics & Spyware Detection | iOS / Android | Forensics toolkit developed by Amnesty International to identify traces of sophisticated mercenary spyware compromises (e.g., Pegasus, Predator). |
| **[Androguard](https://github.com/androguard/androguard)** | [![GitHub stars](https://img.shields.io/github/stars/androguard/androguard?style=social&color=white)](https://github.com/androguard/androguard/stargazers) | Static Analysis & Reverse Engineering | Android (DEX/APK) | Comprehensive reverse engineering, malware analysis, and decompilation framework written in Python for inspecting Android bytecode and structural anomalies. |
| **[Nogotofail](https://github.com/google/nogotofail)** | [![GitHub stars](https://img.shields.io/github/stars/google/nogotofail?style=social&color=white)](https://github.com/google/nogotofail/stargazers) | Network Threat & SSL/TLS Testing | Cross-Platform (Android/iOS) | Google-developed on-path network traffic security testing tool that flags SSL/TLS vulnerabilities, MITM risks, and insecure cleartext data exfiltration. |
| **[APKiD](https://github.com/rednaga/APKiD)** | [![GitHub stars](https://img.shields.io/github/stars/rednaga/APKiD?style=social&color=white)](https://github.com/rednaga/APKiD/stargazers) | Compiler / Packer / Obfuscator Identification | Android (APK) | PEiD-style detection tool that identifies third-party packers, obfuscators, anti-analysis wrappers, and compilers embedded within malicious Android binaries. |
| **[Hypatia](https://github.com/Divested-Mobile/Hypatia)** | [![GitHub stars](https://img.shields.io/github/stars/Divested-Mobile/Hypatia?style=social&color=white)](https://github.com/Divested-Mobile/Hypatia/stargazers) | On-Device Malware Scanner | Android | Real-time, privacy-preserving on-device malware scanner utilizing ClamAV signature databases. Runs fully locally with zero network telemetry or tracking. |
| **[SpyGuard](https://github.com/SpyGuard/SpyGuard)** | [![GitHub stars](https://img.shields.io/github/stars/SpyGuard/SpyGuard?style=social&color=white)](https://github.com/SpyGuard/SpyGuard/stargazers) | Network Stalkerware / Spyware Detection | Cross-Platform (Mobile Network) | Enhanced community fork of TinyCheck designed to detect signs of compromise and stalkerware communication by monitoring outgoing network flows from mobile devices. |
| **[MaintainTeam Hypatia](https://github.com/MaintainTeam/Hypatia)** | [![GitHub stars](https://img.shields.io/github/stars/MaintainTeam/Hypatia?style=social&color=white)](https://github.com/MaintainTeam/Hypatia/stargazers) | Real-Time Anti-Malware Engine | Android | Active community fork of the Divested-Mobile Hypatia scanner delivering enhanced signature feed updates and streamlined UI performance for Android devices. |
| **[ANDRO](https://github.com/AryanVBW/ANDRO)** | [![GitHub stars](https://img.shields.io/github/stars/AryanVBW/ANDRO?style=social&color=white)](https://github.com/AryanVBW/ANDRO/stargazers) | Exploitation & Security Analysis | Android | Android vulnerability assessment and security analysis utility built to identify device misconfigurations, test system exposure, and simulate attack surfaces. |
| **[ShieldApp](https://github.com/beenuar/shieldapp-android)** | [![GitHub stars](https://img.shields.io/github/stars/beenuar/shieldapp-android?style=social&color=white)](https://github.com/beenuar/shieldapp-android/stargazers) | Personal Security Suite & Antivirus | Android | Consumer-grade mobile protection suite combining YARA/heuristic antivirus scanning, on-device deepfake detection, Tor VPN routing, and anti-phishing safeguards. |
| **[AndroDR](https://github.com/yasirhamza/AndroDR)** | [![GitHub stars](https://img.shields.io/github/stars/yasirhamza/AndroDR?style=social&color=white)](https://github.com/yasirhamza/AndroDR/stargazers) | On-Device Endpoint Detection (EDR) | Android | On-device endpoint detection and response (EDR) prototype that actively identifies stalkerware, covert surveillance, and anomalous application behaviors. |
| **[Cybe](https://github.com/cyberlog69/Cybe-App)** | [![GitHub stars](https://img.shields.io/github/stars/cyberlog69/Cybe-App?style=social&color=white)](https://github.com/cyberlog69/Cybe-App/stargazers) | Personal Privacy & Wi-Fi Defense | Android / iOS | Cross-platform privacy and defense app providing Wi-Fi threat scanning (ARP spoofing, SSL stripping), encrypted DNS, phishing link verification, and panic wipe. |

---

## Enterprise vs Open-Source Comparison

When architecting a mobile defense strategy, understand the fundamental trade-offs between commercial enterprise MTD and open-source projects:

| Architectural Requirement | Enterprise MTD (Zimperium, Lookout, Defender) | Open-Source Security (Hypatia, ShieldApp, MVT) |
| :--- | :--- | :--- |
| **MDM / UEM Integration** | Native API connectors (Microsoft Intune, VMware Workspace ONE, Jamf Pro) | None; standalone apps without centralized mobile device management enrollment |
| **Conditional Access Gating** | Real-time risk posture signals block compromised devices from corporate SaaS (Exchange, Slack, Salesforce) | Manual remediation required; cannot enforce network access restrictions automatically |
| **Fleet Forensics & SIEM** | Centralized telemetry ingested into Microsoft Sentinel, Splunk, Datadog, or Falcon XDR | Individual device log exports; requires external manual analysis or custom scripts |
| **Threat Intelligence Feeds** | Hundreds of millions of global endpoints analyzed using proprietary cloud ML behavioral models | Community-curated YARA rules, ClamAV hashes, or public IOC datasets |
| **Employee Privacy Safeguards** | Zero collection of SMS text bodies, photos, browsing history, or personal app contents | Completely local and open source; code is publicly auditable for zero tracking |

---

## How to Contribute

1. Fork this repository.
2. Add or update entries in `README.md` maintaining table formatting, pricing transparency, and accurate star counters.
3. Ensure all links point to authoritative vendor documentation or direct GitHub repositories.
4. Submit a Pull Request with a clear description of changes.

---

## License & Disclaimer

- Community curated — not an endorsement of any commercial platform.
- Always review licensing terms before integrating into commercial products (e.g., GPL-3.0 vs. Apache-2.0 vs. MIT).
