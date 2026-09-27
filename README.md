# Awesome-Email-Security

## Top Email Security Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Anti-Phishing, Spam Filtering, Email Gateway Protection & Security Awareness Training*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Email Security**. These tools help organizations defend against phishing, spam, malware, business email compromise (BEC), and social engineering attacks targeting email infrastructure.



**Examples** include Proofpoint, Mimecast, Abnormal Security, Avanan by Check Point, Microsoft Defender for Office 365, Barracuda Email Protection, IRONSCALES, SpamTitan, FortiMail, and Cisco Secure Email (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom filtering pipelines, and transparent email security — ideal for organizations that need full control over their email gateway without per-user SaaS fees or vendor lock-in.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Proofpoint](https://www.proofpoint.com/)**

  Enterprise email security platform with advanced threat protection, targeted attack protection (TAP), and security awareness training. Defends against phishing, BEC, ransomware, and malware with ML-powered detection.



- **[Mimecast](https://www.mimecast.com/)**

  Cloud email security and cyber resilience platform. Provides targeted threat protection, email continuity, archiving, and awareness training in a unified service.



- **[Abnormal Security](https://abnormalsecurity.com/)**

  AI-native email security platform focused on detecting sophisticated BEC and social engineering attacks that bypass traditional secure email gateways. Uses behavioral AI to baseline normal communication patterns.



- **[Avanan by Check Point](https://www.checkpoint.com/)**

  Cloud email security platform (acquired by Check Point) that protects Microsoft 365 and Google Workspace. API-based architecture with advanced phishing and malware detection.



- **[Microsoft Defender for Office 365](https://www.microsoft.com/en-us/security/business/office-365-defender)**

  Native email security for Exchange Online. Provides anti-phishing, anti-spam, anti-malware, Safe Links, Safe Attachments, and attack simulation training.



- **[Barracuda Email Protection](https://www.barracuda.com/)**

  Email security gateway with AI-powered phishing detection, BEC protection, and account takeover prevention. Available as cloud service or on-premises appliance.



- **[IRONSCALES](https://ironscales.com/)**

  AI-powered email security platform with automated phishing remediation. Uses community-powered threat intelligence and mailbox-level remediation.



- **[SpamTitan](https://www.spamtitan.com/)**

  Email security and spam filtering solution for SMBs and MSPs. Provides anti-spam, anti-virus, anti-phishing, and email archiving with simple deployment.



- **[FortiMail](https://www.fortinet.com/)**

  Fortinet's email security gateway. Protects against spam, malware, phishing, and data leakage with on-premises, cloud, or hybrid deployment options.



- **[Cisco Secure Email](https://www.cisco.com/)**

  Cisco's email security solution (formerly IronPort). Provides inbound and outbound protection with advanced malware analysis, URL filtering, and data loss prevention.



## Open-Source GitHub Projects



- **[Proxmox Mail Gateway](https://www.proxmox.com/en/proxmox-mail-gateway)**

  The leading open-source email security solution. Full-featured mail proxy deployed between firewall and internal mail servers. Features anti-spam (SpamAssassin), anti-virus (ClamAV), object-oriented rule system, message tracking center, spam quarantine with end-user previews, and REST API for 3rd party integration. Version 9.1 (2026) based on Debian 13.5 with SpamAssassin 4.0.2, ClamAV 1.4.4, PostgreSQL 17, and ZFS 2.4. Handles unlimited domains and millions of emails per day. 100% open-source (AGPL v3) with optional enterprise support subscription . **AGPL v3**.



- **[Rspamd](https://github.com/rspamd/rspamd)**

  Advanced, fast, and open-source spam filtering system. The de facto choice for new mail infrastructure in 2026. Features SPF/DKIM/DMARC/ARC verification, 60+ modules, neural network-based filtering, Redis integration, Lua scripting for custom policies, and a built-in Web UI for real-time statistics and management. Multi-threaded architecture handles tens to hundreds of emails per second. Native support for Ubuntu 20.04+, Debian 11+, CentOS/RHEL 8+, Rocky Linux, and FreeBSD . **Apache 2.0**.



- **[SpamAssassin](https://github.com/apache/spamassassin)**

  The original open-source anti-spam framework. Rule-based heuristic engine combining Bayesian filtering, DNSBL checks, phrase matching, and custom rules. Version 4.0.2 released August 2025, still actively maintained. While Rspamd has become the default for new deployments, SpamAssassin remains a solid choice for existing deployments not ready to migrate . **Apache 2.0**.



- **[ClamAV](https://github.com/Cisco-Talos/clamav)**

  Open-source antivirus engine for detecting trojans, viruses, malware, and other malicious threats. Commonly paired with Rspamd or SpamAssassin for email virus scanning. Used by Proxmox Mail Gateway and most self-hosted mail stacks . **GPL v2**.



- **[Gophish](https://github.com/gophish/gophish)**

  Open-source phishing simulation and security awareness training platform. Web-based UI for creating customizable phishing campaigns, tracking user engagement (open rate, click-through rate, credential submission), and generating training reports. Supports Linux, macOS, and Windows with SQLite or MySQL backend. Used by security teams to test employee awareness and identify training gaps . **MIT**.



- **[MailScanner](https://github.com/MailScanner/mailscanner)**

  Open-source email security and spam detection system. Acts as an email gateway and can be combined with SpamAssassin and ClamAV for comprehensive protection. Supports multiple MTAs including Postfix, Sendmail, and Exim .



- **[Bogofilter](https://bogofilter.sourceforge.io/)**

  Bayesian spam filter that classifies mail as spam or ham based on statistical analysis of message content. Lightweight and fast, suitable for integration with mail delivery agents .



- **[Pyzor](https://github.com/SpamExperts/pyzor)**

  Collaborative spam-blocking networked system. Uses distributed checksum clearinghouse (DCC) principles to detect spam by comparing message fingerprints against a shared database .



### Additional Strong Open-Source Options



- **Anti-Spam Tools**: **ASSP** (transparent SMTP proxy with spam filtering), **Scrollout F1** (highly configurable email gateway), **MailScanner** (virus scanner + spam detector) .

- **Security Awareness**: **Phishing Simulator** (full-stack training platform with NLP analysis), **Is This Fraud?** (AI-powered browser extension for real-time phishing detection) .

- **Email Authentication**: **OpenDMARC** (DMARC implementation), **OpenDKIM** (DKIM signing/verification), **SPF** implementations for mail servers.



**Frameworks for building custom systems**: Combine **Rspamd** for the core filtering engine, **ClamAV** for virus scanning, **Proxmox Mail Gateway** for a complete gateway solution, and **Gophish** for security awareness training. Add **Redis** for Rspamd statistics and **PostgreSQL** for persistent storage.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Email security platforms handle sensitive communications; ensure compliance with data protection regulations and email retention policies.

- Self-hosted open-source solutions require proper security hardening, regular rule updates, and monitoring. AI-generated spam in 2026 is adaptive and grammar-perfect — train your filters constantly with your own traffic data .



---



**Made for security engineers, email administrators, IT operations teams, and security awareness trainers.**

Let's make email security more open, transparent, and effective.
