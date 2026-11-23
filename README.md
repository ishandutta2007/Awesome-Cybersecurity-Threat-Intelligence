# Awesome-Cybersecurity-Threat-Intelligence

## Top Cybersecurity & Threat Intelligence Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on CTI Management, Adversary Tracking & Self-Hosted Intelligence Platforms*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cybersecurity & Threat Intelligence**. These tools help security teams collect, structure, analyze, and operationalize threat data—covering everything from commercial intelligence feeds and adversary tracking platforms to open-source TIPs that let you own your intelligence pipeline without per-seat licensing.

**Examples** include Recorded Future, CrowdStrike Falcon Intelligence, Mandiant Advantage, ThreatConnect, MISP, OpenCTI, and IntelOwl (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted threat intelligence management, open-source IOC enrichment, and community-driven intelligence sharing—ideal for security teams seeking data sovereignty and avoiding six-figure enterprise contracts. The open-source landscape is genuinely mature: **MISP** is the de facto standard for intelligence sharing with ATT&CK and TLP galaxies built in , **OpenCTI** provides structured CTI knowledge management with STIX/TAXII interoperability , and **IntelOwl** delivers scalable IOC enrichment across dozens of analyzers .

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Cyber Threat Intelligence (CTI) market is estimated at approximately **$11.5B–$20.1B** and is projected to expand past **$50B+** into the 2030s (15–20% CAGR). The market structure is a **hybrid barbell**: it remains **highly fragmented** across specialized point feeds, dark web monitoring, and boutique IOC providers, while simultaneously experiencing **aggressive concentration and platform consolidation** around major cybersecurity titans (e.g., CrowdStrike, Google Cloud/Mandiant, Mastercard/Recorded Future) that bundle CTI directly into broad enterprise SecOps, SIEM, and XDR platforms.

## SaaS/Hosted Platforms

| Platform | Market Size / Valuation | Starting Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[CrowdStrike Falcon Intelligence](https://www.crowdstrike.com/)** | **~$235B+ Market Cap** (~$5.39B ARR) | **$59.99/device/year** (Falcon Go entry tier; Falcon Intelligence bundle ~$166.56/license) | **15-Day Free Trial** (Full access to core NGAV and threat detection modules; no credit card required) | Adversary intelligence integrated directly with endpoint protection and unified Falcon platform telemetry. |
| **[Mandiant Advantage](https://www.mandiant.com/)** | **$5.4B Valuation** (Acquired by Google; ~$483M+ ARR pre-acquisition) | **~$75,000–$83,000/year** (Standard entry tier; custom contract scope) | **Permanent Free Tier** (Access limited to basic threat actor/malware profiles & CVE data; includes automatic 14-day full feature trial upgrade upon signup) | Threat intelligence backed by Google Cloud and frontline incident response investigations. |
| **[Recorded Future](https://www.recordedfuture.com/)** | **$2.65B Valuation** (Acquired by Mastercard; ~$300M ARR) | **$40,000–$50,000/year** (Single module entry; Microsoft Marketplace Threat User License starts at $50,000/year) | **No Free Tier** (14-to-30 day sales-assisted custom enterprise PoC trial available upon request for qualified organizations) | Real-time commercial intelligence platform aggregating open, deep, and dark web intelligence. |
| **[Flashpoint](https://flashpoint.io/)** | **~$100M ARR** (Venture-backed by Georgian & Greycroft) | **~$57,000/year** (Flashpoint Ignite entry contract median) | **No Free Tier** (Sales-assisted demo and structured enterprise proof-of-concept trial evaluation on request) | Deep and dark web intelligence specialist covering illicit forums, compromised credentials, and ransomware tracking. |
| **[Anomali](https://www.anomali.com/)** | **~$60M–$65M ARR** ($95M+ VC funding) | **~$90,000–$93,000/year** (ThreatStream base enterprise contract average) | **No Free Tier** (14-day enterprise proof-of-concept evaluation available upon sales approval) | Threat intelligence management and security analytics integrating feeds with enterprise SIEM/EDR. |
| **[ThreatConnect](https://threatconnect.com/)** | **~$40.4M ARR** ($22M+ VC funding) | **$45,000/year** (Starting TI Ops platform tier; community API starts at $19/mo) | **Permanent Free Community Tier** (Capped at 1–3 user seats, restricted historical data window, and excludes automated integrations) | Threat intelligence operations platform (TIP) featuring built-in analytics, orchestration, and risk quantification. |
| **[SOCRadar](https://socradar.io/)** | **~$120M–$130M Valuation** (~$30M–$35M ARR; Series B) | **$4,550/year** ($600/month for Advanced Dark Web Monitoring Essential; CTI Essential at $14,750/year) | **Permanent Free Tier** (Restricted to 1 corporate user, 1 corporate domain, 100 auto-discovered digital assets, and excludes API integrations) | Extended threat intelligence (XTI) platform with modular ASM, Dark Web Monitoring, and CTI feeds. |

## Open-Source GitHub Projects

- **[MISP](https://github.com/MISP/MISP)**  
  **The de facto standard open-source threat intelligence sharing platform.** **Free and open standards**—software, data format, and API are all open . **Stores IOCs in a structured manner** with correlation, automated exports for IDS/SIEM (STIX, OpenIOC), and MISP-to-MISP synchronization . **Community-maintained galaxies and taxonomies** include **MITRE ATT&CK, TLP, Exploit-Kit, Ransomware, Threat Actor, and sector-specific models** . **PyMISP** Python library for programmatic access; **MISP modules** extend with expansion, import, and export services . **Latest release: MISP 2.5.47** with PostgreSQL support, AI-assisted workflows, and the Overmind interface . **Best for organizations wanting the most widely adopted intelligence sharing platform** with structured data and community trust groups.

- **[OpenCTI](https://github.com/OpenCTI-Platform/opencti)**  
  **The leading open-source platform for structured cyber threat intelligence knowledge management.** **Created to structure, store, organize, and visualize technical and non-technical information about cyber threats** . **STIX/TAXII native**—designed for interoperability and intelligence sharing . Positioned for teams wanting a modern, graph-based CTI platform that goes beyond IOC storage into knowledge modeling . **Best for organizations wanting a comprehensive CTI knowledge base** with relationship mapping and visualization.

- **[IntelOwl](https://github.com/intelowlproject/IntelOwl)**  
  **The most scalable open-source IOC enrichment platform.** **Integrates dozens of analyzers**—VirusTotal, AbuseIPDB, GreyNoise, Shodan, AlienVault OTX, MISP, and many more . **Enriches files and observables** (IP, domain, URL, hash) via a single API request . **REST API** (Django/Python), built-in GUI with dashboards and visualizations, and **official client libraries** (`pyintelowl`, `go-intelowl`) . **Modular plugin framework**: analyzers (retrieve/generate intel), connectors (export to MISP/OpenCTI), pivots (chain analysis), visualizers, ingestors, and playbooks . **Best for SOC teams wanting to automate common enrichment jobs** without building each integration manually.

- **[Yeti](https://github.com/yeti-platform/yeti)**  
  **Open-source platform at the CTI-DFIR intersection.** **Apache-2.0 licensed**, Python, **1,949 GitHub stars**, actively maintained (pushed 27 days ago) . **"Your Everyday Threat Intelligence"**—focused on making threat intelligence actionable for incident responders and analysts . **Best for teams wanting a lightweight, DFIR-oriented intelligence platform** that bridges threat data and investigation workflows.

### Additional Strong Open-Source Options

- **Threat Bus** — **Dissemination layer for distributing selected indicators to detection systems**. Not a full TIP—it complements MISP or OpenCTI by handling the "last mile" of intelligence distribution. **Recent maintenance activity appears limited**—evaluate project activity before new production deployments [citation:1].

- **TheHive** — **Collaborative incident investigation and case management platform**. Handles cases, alerts, tasks, observables, and workflows; imports from MISP. **⚠️ TheHive 3 and 4 are no longer maintained or publicly distributed**—the latest version is commercially distributed. Not recommended as an open-source TIP [citation:1].

**Frameworks for building custom systems**: Combine **MISP** for intelligence sharing and IOC storage, **OpenCTI** for knowledge management and visualization, and **IntelOwl** for automated enrichment. Use **Threat Bus** to distribute indicators to detection systems if needed—but validate its maintenance status first [citation:1].

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Threat intelligence platforms handle sensitive indicators and adversary data; enforce access controls and validate intelligence quality before operationalizing. **A $0 license does not mean $0 TCO**—deployment, integrations, maintenance, analyst time, and training all count [citation:1].
- **Commercial pricing is opaque and varies significantly.** Recorded Future's Microsoft Marketplace listing shows **$50,000–$100,000/year** depending on license type [citation:7]. ThreatConnect starts at **$45,000** [citation:10]. SOCRadar publishes transparent pricing with a **freemium tier** [citation:12]. **Open-source TIPs (MISP, OpenCTI) eliminate license costs but shift burden to engineering**—the real question is whether your team has the capacity to operate, secure, and maintain the platform as intelligence volume and integrations grow [citation:1]. **TheHive is no longer an open-source option**—versions 3 and 4 are unmaintained, and the current version is commercial [citation:1]. Validate whether you need managed intelligence (Recorded Future, Mandiant) or a self-hosted pipeline (MISP, OpenCTI, IntelOwl) before committing.

---

**Made for SOC analysts, CTI researchers, and organizations building intelligence-driven defense.**  
Let's make cybersecurity and threat intelligence more open, structured, and actionable.
