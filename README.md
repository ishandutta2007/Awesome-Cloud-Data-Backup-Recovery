# Awesome-Cloud-Data-Backup-Recovery

# Top Cloud Data Backup & Recovery Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Backup as a Service (BaaS), Disaster Recovery & Cyber-Resilient Data Protection*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Data Backup & Recovery**. These tools help organizations protect workloads across on-premises, cloud, and SaaS environments—covering immutable backups, automated recovery orchestration, ransomware detection, and long-term retention for compliance.

**Examples** include Druva, Veeam Cloud Connect, Acronis Cyber Protect, Datto SIRIS, Commvault, Cohesity, Backblaze, Carbonite, Rubrik, and Zoho Backup (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted backup engines, disaster recovery orchestration, and deduplicated storage—ideal for SREs, platform engineers, and organizations seeking transparent, vendor-neutral resilience without per-TB cloud billing surprises.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Druva](https://www.druva.com/)** | Cloud-native data protection with agentless backup, global deduplication, and automated cloud DR. Business, Enterprise, and Elite tiers differ by included features (cross-cloud backup, cyber recovery, GovCloud are higher-tier or add-ons). Billed per TB/month after deduplication [citation:2]. | Enterprise tier: from ~€191/TB/month (approx. $210 USD) via reseller; M365 from ~€2.47/user/month [citation:12] | No published free tier; trial available via sales |
| **[Veeam Cloud Connect](https://www.veeam.com/)** | Multi-tenant platform for service providers to deliver Veeam-powered off-site backup and DRaaS. Licensed per protected workload (PPU). Tenants with rental licenses consume zero points for backup/backup copy; subscription/perpetual tenants consume 5 PPU per VM [citation:13]. | Free platform; Veeam backup licenses required (VCSP rental points apply) | Free to deploy; 14-day trial available via service providers |
| **[Acronis Cyber Protect Cloud](https://www.acronis.com/)** | Cyber protection platform combining backup, disaster recovery, and AI-based ransomware detection. Service providers choose per-workload or per-GB pricing; minimum monthly commitment of USD 250 for hosted storage Tier 1 [citation:4]. | Per-workload: Server ~$40/month (example); VM + Advanced Backup ~$15/month (example) [citation:4] | Free licensing model for onboarding (limited functionality); pay-as-you-go from there [citation:14] |
| **[Datto SIRIS](https://www.datto.com/)** | Business continuity and disaster recovery appliance with local and cloud virtualization, screenshot verification, and ransomware detection. Pricing based on data usage (2.5:1 sizing ratio) and server count. SIRIS 6 pricing starts at approximately $1,095 [citation:5][citation:15]. | From ~$995–$1,095 (varies by model, storage, retention, contract length) [citation:5][citation:15] | No free tier; trial via partner program |
| **[Commvault Complete Backup & Recovery](https://www.commvault.com/)** | Enterprise data protection with immutable backups, air-gapped copies, and cleanroom recovery. Command Center provides centralized policy and license management. | Physical server: ~$1,885 per instance; VM: ~$2,729 per VM; Endpoint: ~$120 per user [citation:6] | No free tier; trial available via sales |
| **[Cohesity DataProtect](https://www.cohesity.com/)** | AI-powered data protection with immutable snapshots, threat detection, and DataProtect as a Service (DPaaS) for fully managed cloud backup. DPaaS bundles infrastructure, software, and support into a per-TB subscription [citation:7]. | DPaaS: $200–$500+ per TB annually (based on retention, replication, SLA) [citation:7] | No free tier; trial available via sales |
| **[Rubrik Cloud Data Management](https://www.rubrik.com/)** | Cloud data management platform with immutable backups, anomaly detection, and orchestrated recovery. Available via Azure Marketplace with long-term billing. | Marketplace listing starting at $90,000/month (enterprise scale) [citation:10] | No free tier; trial available via sales |
| **[Backblaze B2](https://www.backblaze.com/)** | Object storage for backup and archive. Transparent pay-as-you-go pricing: $6.95/TB/month storage, first 10 GB free, free egress up to 3x average stored data [citation:8]. | $6.95/TB/month; egress beyond 3x: $0.01/GB [citation:8] | First 10 GB storage free; free egress up to 3x stored data |
| **[Carbonite](https://www.carbonite.com/)** | Server and endpoint backup with cloud storage, granular restore, and compliance support. Core, Power, and Ultimate tiers based on number of computers and servers [citation:9]. | Power (1 server + 25 computers, 500 GB): $50/month or $599.99/year [citation:9] | No free tier; 30-day money-back guarantee typically offered |
| **[Zoho Backup](https://www.zoho.com/)** | Data backup for Zoho CRM and Bigin. Administrators can initiate on-demand backups; recurring backups available as add-on purchases [citation:1][citation:11]. | Free plan: $10 per backup; Paid plans: 2 free backups/month, $10 per additional [citation:11] | Free edition: pay-per-backup only; Paid editions: 2 free backups/month [citation:11] |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Restic](https://github.com/restic/restic)** | [![Stars](https://img.shields.io/github/stars/restic/restic?style=social&color=white)](https://github.com/restic/restic/stargazers) | Fast, secure, deduplicated backup tool with encryption and support for S3, GCS, Azure Blob, SFTP, and local storage. CLI-first, widely used as a self-hosted BaaS foundation. |
| **[BorgBackup](https://github.com/borgbackup/borg)** | [![Stars](https://img.shields.io/github/stars/borgbackup/borg?style=social&color=white)](https://github.com/borgbackup/borg/stargazers) | Deduplicating, compressing, authenticated backup tool with encryption. Supports local, SSH, and cloud storage backends; mature and battle-tested. |
| **[Velero](https://github.com/vmware-tanzu/velero)** | [![Stars](https://img.shields.io/github/stars/vmware-tanzu/velero?style=social&color=white)](https://github.com/vmware-tanzu/velero/stargazers) | Kubernetes backup and restore tool for cluster resources and persistent volumes. Supports AWS, Azure, GCP, and on-premises storage; includes schedules and pre/post hooks. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[ReaR (Relax-and-Recover)](https://github.com/rear/rear)** | [![Stars](https://img.shields.io/github/stars/rear/rear?style=social&color=white)](https://github.com/rear/rear/stargazers) | Linux disaster recovery framework producing bootable rescue images; supports Bacula, Borg, Duplicity, rsync, and many enterprise backup backends. |
| **[Duplicati](https://github.com/duplicati/duplicati)** | [![Stars](https://img.shields.io/github/stars/duplicati/duplicati?style=social&color=white)](https://github.com/duplicati/duplicati/stargazers) | Open-source backup software with web-based management, encryption, and support for S3, SFTP, WebDAV, and cloud storage destinations. |
| **[Kopia](https://github.com/kopia/kopia)** | [![Stars](https://img.shields.io/github/stars/kopia/kopia?style=social&color=white)](https://github.com/kopia/kopia/stargazers) | Fast, secure backup/restore tool with deduplication, encryption, and support for S3, Azure, GCS, and local storage. Includes server mode and web UI. |

**Frameworks for building custom systems**: Combine **Restic** or **BorgBackup** for encrypted, deduplicated backup storage, **Velero** for Kubernetes workload protection, **Kopia** for cross-platform backup with a web UI, and **ReaR** for bare-metal Linux recovery—creating a fully self-hosted BaaS/DRaaS stack on commodity infrastructure or cloud object storage.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Backup and recovery tools handle sensitive production data; enforce encryption at rest and in transit, least-privilege access, and regular restore testing.
- Self-hosted open-source solutions require capacity planning, off-site replication, and immutable storage strategies to protect against ransomware; always validate RTO/RPO against business requirements.

---

**Made for SREs, platform engineers, backup administrators, and organizations building cyber-resilient infrastructure.**  
Let's make cloud data backup and recovery more open, automated, and provable.
