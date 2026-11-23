# Awesome-Cybersecurity-Threat-Intelligence

# Top Cybersecurity & Threat Intelligence Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on CTI Management, Adversary Tracking & Self-Hosted Intelligence Platforms*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cybersecurity & Threat Intelligence**. These tools help security teams collect, structure, analyze, and operationalize threat data—covering everything from commercial intelligence feeds and adversary tracking platforms to open-source TIPs that let you own your intelligence pipeline without per-seat licensing.

**Examples** include Recorded Future, CrowdStrike Falcon Intelligence, Mandiant Advantage, ThreatConnect, MISP, OpenCTI, and IntelOwl (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted threat intelligence management, open-source IOC enrichment, and community-driven intelligence sharing—ideal for security teams seeking data sovereignty and avoiding six-figure enterprise contracts. The open-source landscape is genuinely mature: **MISP** is the de facto standard for intelligence sharing with ATT&CK and TLP galaxies built in , **OpenCTI** provides structured CTI knowledge management with STIX/TAXII interoperability , and **IntelOwl** delivers scalable IOC enrichment across dozens of analyzers .

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Recorded Future](https://www.recordedfuture.com/)**  
  **The largest commercial threat intelligence platform.** Combines open web, dark web, and technical sources into real-time intelligence. **Microsoft Marketplace pricing**: Threat User License at **$50,000/year**; custom plans at **$100,000/year** . Positioned for enterprises wanting comprehensive, analyst-ready intelligence without building collection infrastructure.

- **[CrowdStrike Falcon Intelligence](https://www.crowdstrike.com/)**  
  Threat intelligence integrated with the Falcon platform. **CDW-G listing**: 12-month Falcon Intelligence Bundle subscription at **~$166.56 per license** (25,000–49,999 license band) . Positioned for existing CrowdStrike customers wanting adversary intelligence alongside endpoint protection.

- **[Mandiant Advantage](https://www.mandiant.com/)**  
  **Google-owned threat intelligence with frontline adversary knowledge.** Subscription-based pricing with tiered plans varying by monitoring level, response capabilities, and asset count—typically per user or per protected asset, with annual or multi-year agreements . Positioned for organizations wanting intelligence from the team that responds to major breaches.

- **[ThreatConnect](https://threatconnect.com/)**  
  **Threat intelligence platform with a free edition and paid tiers starting at $45,000.** Features, functionality, and deployment model (private cloud, public cloud, or on-premises) determine the price . Positioned for teams wanting a TIP with built-in analytics and orchestration.

- **[SOCRadar](https://socradar.io/)**  
  **Extended threat intelligence with published pricing and a freemium tier.** **Cyber Threat Intelligence Essential: $14,750/year** (or $1,625/month); **Advanced Dark Web Monitoring Essential: $4,550/year**; **Business: $9,100/year** . **SOC 2 Type 2 and ISO/IEC 27001 certified** . Positioned for mid-market teams wanting transparent pricing across modules (ASM, Brand Protection, CTI, Dark Web, Supply Chain).

- **[Anomali](https://www.anomali.com/)**  
  Threat intelligence and security analytics platform. **Quote-based pricing** scoped to usage and team size; free trial available . Positioned for enterprises wanting SIEM-adjacent intelligence analytics.

- **[Flashpoint](https://flashpoint.io/)**  
  **Deep and dark web intelligence specialist.** Core packages include Cyber Threat Intelligence (illicit groups/sites, tailored reports, API access, account takeover credentials, vulnerability intelligence), Vulnerability, and Physical Security . Claims **482% ROI in 6 months** and **$500M fraud loss avoided per year** . Positioned for teams needing illicit community visibility.

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
