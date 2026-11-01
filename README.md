# Awesome-Cybersecurity-Application-Development-Platform

# Awesome-Cybersecurity-Application-Development-Platform

# Awesome-Cybersecurity-Application-Development-Platform
**Top Cybersecurity Application Development Platform (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Security App Marketplaces, Low-Code Automation, Serverless Security Functions & Self-Hosted SOAR*
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cybersecurity Application Development Platforms**. These tools enable security teams to build, deploy, and share custom applications, workflows, and integrations on top of security platforms—from fully managed app marketplaces with no-code automation to self-hosted SOAR engines that give organizations control over their security orchestration.

**Examples** include CrowdStrike Falcon Foundry, Palo Alto Cortex XSOAR, Splunk SOAR, SentinelOne Singularity Marketplace, Microsoft Security Copilot Ecosystem, Torq, Tines, Elastic Security, Rapid7 Insight, and AWS Security Hub (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted security automation, app development, and open SOAR infrastructure. **Critical note**: The open-source landscape is anchored by **Shuffle**—a no-code SOAR platform with a genuine free tier and self-hosted option . **Wazuh + Cortex + TheHive** forms a component-rich open-source SOAR-like stack . However, no open-source project matches CrowdStrike Foundry's native Falcon console integration or SentinelOne's serverless FaaS hosting.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[CrowdStrike Falcon Foundry](https://developer.crowdstrike.com/foundry/)**
  **Application development platform** for building custom apps natively inside the Falcon console. **Features**: UI extensions (panels, tabs, cards on detection/incident/host pages), serverless functions in Python or Go, LogScale queries for dashboards, Fusion SOAR workflow templates, RTR scripts, and API integrations. **Pricing**: Requires **Falcon Foundry entitlement**—contact CrowdStrike representative; no public self-serve pricing. **Free tier**: Not available; entitlement tied to Falcon subscription. **Best for**: CrowdStrike customers wanting to extend the Falcon console with custom UI, workflows, and data—**trade-off**: deep lock-in to Falcon ecosystem; requires Foundry entitlement.

- **[Palo Alto Cortex XSOAR](https://www.paloaltonetworks.com/cortex/cortex-xsoar)**
  **Security orchestration, automation, and response** platform with playbook development. **Features**: Integrated threat intelligence management, War Room collaboration with full audit trails, MSSP multi-tenant licensing. **Pricing**: **MSSP license from ~$16,600 per user**; Enterprise packages have high entry costs. Palo Alto naming **Cortex AgentiX** as XSOAR's next generation, licensed per user with metered compute units. **Critical note**: Professional services for XSOAR are **end-of-sale since February 2026**; **air-gapped support removed in v8**; AgentiX is **cloud-only**—transition risk for traditional XSOAR buyers is elevated. **Free tier**: Not specified; enterprise sales-led. **Best for**: Palo Alto-centric organizations accepting the AgentiX transition—**trade-off**: high entry cost; air-gap loss; ecosystem binding.

- **[SentinelOne Singularity Marketplace](https://www.sentinelone.com/platform/singularity-marketplace/)**
  **No-code automation ecosystem** for extending Singularity XDR. **Features**: Bite-sized one-click apps for intelligence, automation, and data integrations; hosted on **Nexus** serverless FaaS platform; no on-prem infrastructure required; 2-way actionable data between SentinelOne and connected tools. **Pricing**: **Quote-only**; bundled with Singularity platform. N-able's Singularity Complete package is purchasable through **AWS Security Hub Extended with pay-as-you-go pricing**—configure from the Security Hub console. **Free tier**: None. **Best for**: SentinelOne customers wanting SOAR-like automation without dedicated SOAR infrastructure—**trade-off**: apps must run on Nexus; limited to API-enabled integrations.

- **[Torq](https://torq.io/)**
  **AI SOC security platform** with agentic automation. **Features**: **300+ pre-built integrations** and **4,000+ pre-built steps**; bidirectional integrations with CrowdStrike, Okta, and others; public REST API and MCP client support. **Pricing**: **Quote-only; annual contracts only**; **no free tier, no self-serve trial**; AWS Marketplace purchases run on **12-month contracts**. Reviewers note Torq integrates case management **without extra charges**, unlike XSOAR. **Free tier**: None. **Best for**: enterprises wanting aggressive autonomous remediation—**trade-off**: ~1 month implementation; no self-serve evaluation.

- **[Tines](https://www.tines.com/)**
  **Workflow automation platform** for security teams. **Features**: No-code workflow builder; unlimited integrations on all tiers; AI runtime credits or bring-your-own model on paid tiers. **Pricing**: **Community edition (forever free)**—**unlimited viewers, unlimited parallel runs, unlimited integrations, SSO, 1 builder, 3 live workflows**, and a **one-time $50 AI allowance**; **cannot bring your own AI model**. **Starter edition** adds multiple builders, **1M monthly events, 7-day retention**; paid tiers quote-based. **Free tier**: Yes, Community with 3 flows. **Best for**: teams wanting to experiment with security automation without a sales call—**trade-off**: Community limited to 1 builder and 3 flows.

- **[Microsoft Security Copilot Ecosystem](https://www.microsoft.com/security/copilot)**
  **Security Store and partner agent ecosystem** within Security Copilot. **Features**: Security Store for partner agents; agents access Defender, Sentinel, Intune, and Entra data after Global Admin approval; separate billing for Security Store subscriptions (partner fees) and **Security Compute Unit (SCU)** consumption. **Pricing**: **SCU capacity**—provisioned capacity billed **hourly in fixed clock blocks** (unused SCUs expire at hour end, no rollover); **overage capacity** billed on demand with configurable limits; **M365 E5/E7 customers** get auto-provisioned default capacity. **Free tier**: Included capacity for M365 E5/E7. **Best for**: Microsoft security customers wanting to extend Copilot with partner agents—**trade-off**: dual billing (SCU + partner subscription); hourly provisioning requires usage modeling.

- **[Splunk SOAR](https://www.splunk.com/)**
  **Security orchestration and automation** within Splunk. **Features**: Playbook automation, case management, app development via SDKs and APIs. **Pricing**: Quote-only; enterprise contracts. **Free tier**: None. **Best for**: Splunk customers wanting SOAR integrated with their SIEM—**trade-off**: enterprise pricing; playbook migration from competitors often requires complete redesign.

- **[Elastic Security](https://www.elastic.co/security)**
  **SIEM and security analytics** with serverless pricing. **Features**: Prebuilt detection rules, endpoint protection (Elastic Defend), AI Assistant, Workflows for scripted automation and AI agents. **Pricing**: **Serverless ingest from $0.09/GB** (Essentials) or **$0.11/GB** (Complete); retention from **$0.017/GB/month**; **no per-endpoint fees as of March 2026**; **50 GB egress free**, then $0.05/GB. Workflows: **10,000 executions free**, then **$0.0108/execution** (Essentials) or **$0.025** (Complete); Agent Builder **$0.025/execution**. **Free tier**: Trial available; no permanent free tier. **Best for**: teams wanting usage-based SIEM without per-endpoint costs—**trade-off**: source-available license (Elastic 2.0/SSPL), not OSI open source.

- **[Rapid7 Insight Platform](https://www.rapid7.com/)**
  **Security analytics platform** with vulnerability management and SIEM. **Features**: InsightVM with Active Risk Score, automated remediation, Jira/ServiceNow integration. **Pricing**: **Subscription per asset**; Vendr median **$36,678**; professional services add **10–20%**; annual escalation typically **3–7%**. Bundling multiple products (InsightVM + InsightIDR) unlocks volume discounts. **Free tier**: None. **Best for**: teams wanting vulnerability management with risk scoring—**trade-off**: asset-based pricing; negotiate escalation caps.

- **[AWS Security Hub](https://aws.amazon.com/security-hub/)**
  **Unified cloud security** with per-resource pricing. **Features**: Essentials plan includes risk analytics, vulnerability management, CSPM, and response management; threat analytics add-on powered by GuardDuty; Lambda code scanning add-on powered by Inspector. **Pricing**: **Per resource unit**—EC2 instance = 1 unit; Lambda = 1/12; ECR image = 1/18; IAM user/role = 1/125; threat analytics **~¥35.30 per million events** (Beijing region). **Free tier**: **30-day free trial** with essentials plan capabilities; add-ons excluded. **Best for**: AWS-centric organizations wanting consolidated security posture—**trade-off**: per-resource pricing scales with AWS footprint.

## Open-Source GitHub Projects

- **[Shuffle](https://github.com/Shuffle/Shuffle)**
  **Open-source SOAR platform** (AGPL-3.0) — **the most accessible open-source security automation platform** with a genuine free tier and self-hosted option. **Features**: **No-code workflow automation engine**; visual workflow editor with pre-built application connectors—rapid playbook construction without programming expertise; **50 apps** on free tier, **unlimited** on Scale; **10 workflows** on free, unlimited on Scale; **5 users** on free, unlimited on Scale; **multi-tenant** (max 3 tenants on free); on-prem, hybrid, or cloud deployment. **Tech stack**: Python, Go. **Deploy**: Self-hosted or Shuffle Cloud. **Trade-off**: **Audit logging requires Scale tier**; execution retention only 1 month on free; 5-user limit on free tier. **Best for**: teams wanting to start security automation without a sales call—the most pragmatic open-source SOAR entry point.

- **[Wazuh + Cortex + TheHive Stack](https://wazuh.com/)**
  **Component-rich open-source SOAR-like architecture** — **the modular alternative to all-in-one orchestrators**, combining mature projects for detection, enrichment, and case management. **Features**: **Wazuh** for host and network detection (HIDS/SIEM); **Cortex** for indicator enrichment through modular analyzers; **TheHive** for structured case management. An academic comparative study (2026) directly evaluated this stack against Shuffle using identical real-world attack data from T-Pot honeypots and FortiGate firewalls, measuring playbook success rate, response latency, false-positive handling, integration effort, and resource consumption. **Tech stack**: Per component (Wazuh, Cortex, TheHive). **Deploy**: Self-hosted (distributed architecture). **Trade-off**: **More integration effort** than Shuffle's all-in-one approach; three separate projects to maintain. **TheHive 3/4 is no longer maintained**—latest version commercially licensed; evaluate Cortex and Wazuh independently. **Best for**: teams wanting detection, enrichment, and case management from separate mature projects—willing to accept integration complexity for component flexibility.

### Additional Strong Open-Source Options

- **Cortex** — Observable analysis and active response engine (license per repo). Modular analyzers for enrichment; part of the Wazuh + Cortex + TheHive stack. **Note**: **Enrichment component**, not a full SOAR platform. **Best for**: teams wanting indicator enrichment within a modular stack.
- **TheHive (legacy)** — Case management platform (AGPL-3.0 for v3/v4). **Note**: **TheHive 3 and 4 are no longer maintained or publicly distributed**—latest version is commercially licensed. **Do not adopt for new deployments.**
- **No mature open-source security app marketplace exists.** CrowdStrike Foundry, SentinelOne Marketplace, and Microsoft Security Store are proprietary ecosystems with no open-source equivalents. **Shuffle** provides the automation layer but not marketplace distribution and monetization.

**Frameworks for building custom systems**: Combine **Shuffle** for workflow automation with **Wazuh** for detection, **Cortex** for enrichment, and a maintained case management tool—creating a composable open-source security automation stack. **None of these match CrowdStrike Foundry's native console integration or SentinelOne's serverless FaaS marketplace**, but for core automation and app development, the open-source options are functional.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cybersecurity application development platforms handling security credentials and automation logic must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls.
- **The "native app platform" vs. "SOAR" vs. "workflow automation" vs. "modular stack" distinction is critical.** **CrowdStrike Foundry** and **SentinelOne Singularity Marketplace** are **native app platforms**—they extend the parent security product with custom UI and serverless functions. **Cortex XSOAR, Splunk SOAR, and Torq** are **SOAR platforms**—they orchestrate security operations with playbooks. **Tines** is **workflow automation**—general-purpose security workflows without full SOAR case management. **Shuffle** is **open-source SOAR**—the free alternative to commercial SOAR. **Wazuh + Cortex + TheHive** is a **modular stack**—component-rich but requiring integration effort. **Choose based on whether you need native product extension, full SOAR, lightweight automation, or modular flexibility.**
- **Cortex XSOAR transition risk is material in 2026.** Professional services are **end-of-sale since February 2026**; **air-gapped support is removed in v8**; **Cortex AgentiX is cloud-only**. Organizations requiring air-gap or on-prem must evaluate alternatives. **Do not commit to XSOAR without accepting the AgentiX migration path.**
- **Torq has no free tier and no self-serve trial.** Annual contracts only; AWS Marketplace purchases run 12-month terms. **Evaluation requires a demo request and sales engagement.**
- **Tines Community is the most generous free tier**—unlimited viewers, parallel runs, and integrations, with 1 builder and 3 live workflows. **The trade-off**: cannot bring your own AI model on Community; one-time $50 AI allowance.
- **Microsoft Security Copilot SCU provisioning is hourly with no rollover.** Unused SCUs expire at the end of each clock hour—you pay for provisioned capacity whether used or not. **Model your baseline workload carefully before provisioning.**
- **Elastic Security is source-available, not OSI open source.** Elastic License 2.0/SSPL restrictions apply. **Verify license compatibility before embedding in commercial products.**
- **TheHive 3/4 is no longer maintained.** The Wazuh + Cortex + TheHive stack reference uses a legacy component—**evaluate a maintained case management alternative before adopting this architecture.**
- **Pricing opacity varies.** CrowdStrike Foundry requires entitlement (quote-only). Cortex XSOAR, Torq, Splunk SOAR, and SentinelOne require sales contact. Tines publishes free and starter tiers. Elastic publishes serverless per-GB pricing. AWS Security Hub publishes per-resource pricing. Rapid7 publishes per-asset subscription with Vendr benchmarks.
- Self-hosted open-source solutions require proper infrastructure (PostgreSQL/Redis for Shuffle; distributed components for Wazuh stack), security hardening, and ongoing maintenance. **Security automation platforms have privileged access to security tools and credentials**—ensure your deployment meets your organization's security standards before connecting production systems.

---

**Made for security engineers, SOC teams, and organizations building transparent security automation solutions.**
Let's make Cybersecurity Application Development Platforms more open, data-driven, and automation-friendly.
