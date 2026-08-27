# Awesome-SaaS-Security-Posture-Management

# Awesome-SaaS-Security-Posture-Management

## Top SaaS Security Posture Management (SSPM) Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on SaaS Configuration Security, Identity Risk, OAuth/Shadow IT, Misconfiguration Detection & Continuous Compliance Across Business Applications*
**Last updated: August 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **SaaS Security Posture Management (SSPM)**. These systems continuously assess the security configuration of SaaS applications (Microsoft 365, Google Workspace, Salesforce, Slack, etc.), surface misconfigurations, identity and OAuth risks, and help reduce the attack surface of the business application estate.

**Examples** include Adaptive Shield (CrowdStrike Falcon Shield), Obsidian Security, Wing Security, AppOmni, Netskope SSPM, Grip Security, Valence Security, Palo Alto Prisma SaaS / SSPM, Spin.AI, Reco, DoControl, and BetterCloud (the category leaders).

**Open-source emphasis**: Full commercial SSPM platforms have limited pure open-source equivalents. Emerging projects such as **Aperio** and the **Open SSPM Spec** provide building blocks for posture checks, OAuth inventory, and SIEM-native detection. This section lists the most relevant open options.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Adaptive Shield / CrowdStrike Falcon Shield](https://www.crowdstrike.com/)**  
  SSPM capability (acquired Adaptive Shield) integrated into the CrowdStrike Falcon platform, covering configuration posture, compliance, and app hardening across a broad SaaS catalog.

- **[Obsidian Security](https://www.obsidiansecurity.com/)**  
  SaaS security platform combining posture management with identity-aware threat detection and activity analysis for mature SOC teams.

- **[Wing Security](https://wing.security/)**  
  SSPM and SaaS discovery platform strong on shadow IT, third-party app inventory, and supply-chain style risk across the SaaS estate.

- **[AppOmni](https://appomni.com/)**  
  Deep configuration and posture management for critical enterprise SaaS (Salesforce, Workday, ServiceNow, M365, etc.), widely used for audit-grade governance.

- **[Netskope SSPM](https://www.netskope.com/)**  
  SaaS security posture capabilities within the broader Netskope Security Service Edge (SSE) portfolio, alongside CASB and data protection.

- **[Grip Security](https://www.grip.security/)**  
  SaaS security platform focused on discovering and securing the full SaaS estate, including shadow SaaS identified via identity and other signals.

- **[Valence Security](https://www.valence.security/)**  
  SSPM oriented toward SaaS-to-SaaS integrations, OAuth scopes, and collaborative remediation of third-party app risk.

- **[Palo Alto Prisma SaaS / SSPM](https://www.paloaltonetworks.com/)**  
  SaaS security and posture management within the Prisma / SaaS Security portfolio for configuration and data risk visibility.

- **[Spin.AI](https://www.spin.ai/)**  
  SaaS security platform with posture, data protection, and backup-oriented capabilities for Microsoft 365 and Google Workspace.

- **[Reco](https://www.reco.ai/)**  
  AI-driven SaaS security platform analyzing user behavior, sharing patterns, and posture risks with an emphasis on low-noise findings.

- **[DoControl](https://www.docontrol.io/)**  
  SaaS data and posture security platform with no-code workflows for governance, access control, and automated response.

- **[BetterCloud](https://www.bettercloud.com/)**  
  SaaS operations and security platform focused on automated management, policy enforcement, and posture across business applications.

## Open-Source GitHub Projects
- **[Aperio](https://github.com/writer/aperio)**  
  Open-source SSPM / SaaS detection & response project aimed at SIEM-native teams: detects posture risks, inventories OAuth/shadow IT, and streams normalized findings into existing security stacks (connectors for GitHub, Slack, Google Workspace, Okta, M365, and more).

- **[Open SSPM Spec](https://github.com/open-sspm/open-sspm-spec)**  
  Open, versioned specification for SSPM compliance rulesets and profiles (YAML + JSON Schema, Rego checks) that tools can evaluate — a foundation for portable posture benchmarks.

- **[SaaS configuration audit scripts and checkers](https://github.com/)**  
  Community scripts that use official APIs (Microsoft Graph, Google Admin, Salesforce, etc.) to export and evaluate security-relevant settings.

- **[OAuth and third-party app inventory tools](https://github.com/)**  
  Open utilities that enumerate authorized OAuth applications and scopes across identity providers and major SaaS platforms.

- **[CIS and benchmark implementations for SaaS](https://github.com/)**  
  Open mappings and automated checks derived from CIS benchmarks and similar hardening guides for Okta, M365, Google Workspace, and others.

- **[Policy-as-code for SaaS settings (Rego/OPA)](https://github.com/)**  
  Examples of evaluating SaaS configuration exports against Open Policy Agent policies for continuous posture assessment.

- **[SIEM content packs for SaaS logs](https://github.com/)**  
  Open detection rules and dashboards (Sigma, Elastic, Splunk, etc.) that surface suspicious SaaS activity and configuration changes.

- **[Shadow IT discovery from identity and DNS signals](https://github.com/)**  
  Open approaches to discovering unsanctioned SaaS usage from SSO logs, browser, or network telemetry.

- **[Remediation runbook and automation prototypes](https://github.com/)**  
  Scripts and workflows (often tied to ITSM or chatops) that help close common SaaS misconfigurations once detected.

- **[Multi-SaaS inventory and CMDB sync open tools](https://github.com/)**  
  Lightweight open projects that keep a local inventory of SaaS tenants, apps, and high-risk settings for internal reporting.

### Additional Strong Open-Source Options
- Combining Aperio (or similar) with an open SIEM (Wazuh, Security Onion, ELK) for a self-hosted detection loop.
- Using official SaaS APIs + scheduled jobs + OPA/Rego for continuous configuration baselines.
- Open identity security tools (e.g. around Entra ID / Okta) that complement SSPM findings.
- Browser and endpoint signals (where privacy-compatible) to improve shadow SaaS discovery.
- Community checklists and hardening guides published as machine-readable rules.

**Frameworks for building custom systems**: Start with API-based exporters for your critical SaaS apps, evaluate settings against the **Open SSPM Spec** or CIS-derived Rego policies, inventory OAuth apps, and forward findings to your SIEM. **Aperio** can serve as a more complete open detection-and-response layer. This approach suits security teams that already operate a strong SIEM/SOAR stack and want ownership of the logic. Broad multi-app coverage, deep configuration models, automated remediation, and continuous vendor research remain the strengths of commercial SSPM platforms (AppOmni, Adaptive Shield/Falcon Shield, Obsidian, Wing, Grip, Valence, DoControl, etc.).

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- SSPM tools require privileged access to SaaS admin APIs and identity systems. Open-source projects must be deployed with strong secret management, least privilege, and audit logging. Misconfiguration of the security tool itself can create new risks. Always test in non-production tenants first and align with your identity, privacy, and change-management policies.
- No tool replaces solid SaaS admin hygiene, MFA, and least-privilege access design.

---
**Made for security, identity, and SaaS operations teams defending the business application layer.**
Let's make SaaS posture more transparent, measurable, and community-driven where possible.
