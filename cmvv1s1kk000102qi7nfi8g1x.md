---
title: "The A-Z Weekly Wrap: 30th October 2026"
seoTitle: "Azure Weekly Wrap: 30th Oct 2026"
seoDescription: "Latest Azure platform updates for 30th October 2026, covering key announcements across networking, security, compute, databases, and hybrid mgmt."
datePublished: 2026-10-30T14:08:21.995Z
cuid: cmvv1s1kk000102qi7nfi8g1x
slug: weekly-wrap-30102026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/ce646f06-deda-4a39-9b21-a21667a58947.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/521b7737-da6c-4394-b018-4de51597b719.jpg
tags: azure, security, databases, devops, networking, containers, update, compute, atozazure

---

Welcome to this week’s atozazure weekly wrap for the 30 October 2026. Below are all the key platform changes, additions and retirements for the past week.

## Compute & Storage

- **Item-Level Recovery for Azure VMs with Premium SSD v2 and Ultra Disks** *(Generally Available)*\
  Granular single-file and folder-level restore capabilities are now supported across virtual machines backed by Premium SSD v2 and Ultra Disks with both 512-byte and 4 KB logical sector configurations. This eliminates the necessity of restoring entire disk volumes for targeted operational recovery, substantially lowering operational recovery time objectives (RTO) and egress storage costs in **Azure Backup**.
- **ABFS Vectored Read for Azure Data Lake Storage** *(Generally Available)*\
  Compatible big data and distributed analytics runtimes can now issue non-contiguous, batched asynchronous vector read requests against target object stores. This significantly reduces overall storage request overhead and network round-trips for selective columnar and analytical queries hosted on **Azure Data Lake Storage Gen2**.
- **Automatic Zone Balance for Virtual Machine Scale Sets** *(Generally Available)*\
  Autonomous cross-zone distribution monitoring and dynamic node rebalancing have been integrated directly into scalable compute topologies. This mitigates infrastructure drift and bolsters zonal resilience during degradation events without manual rebalancing interventions across **Azure Virtual Machine Scale Sets**.

## Networking & Security

- **Keyless TLS on Application Gateway with Managed HSM** *(Generally Available)*\
  Hardware-isolated cryptographic offloading is now operational for layer-7 ingress traffic, completing TLS handshake signatures directly inside dedicated FIPS 140-2 Level 3 cryptographic boundaries without exporting private keys. This reinforces strict zero-trust and digital sovereignty perimeters for ingress endpoints managed through **Azure Application Gateway** and **Azure Key Vault Managed HSM**.
- **Service Tag Matching for Azure Front Door Premium WAF** *(Generally Available)*\
  Custom Web Application Firewall inspection logic can now incorporate native Microsoft service tag definitions within rule criteria. This simplifies edge security governance and perimeter routing enforcement by dynamically maintaining Microsoft-managed IP ranges within **Azure Front Door**.
- **Disable VNet Peering Route (DPR)** *(In Preview)*\
  Granular routing control now allows platform engineers to selectively suppress default system-generated peering routes across individual subnet route tables. This enables deterministic transit hub enforcement and strict egress traffic inspection patterns through central network virtual appliances in **Azure Virtual Network**.
- **Azure DNS Integration with Traffic Manager Linked Records** *(Generally Available)*\
  Direct record linking enables native DNS-based traffic steering and health probing without provisioning intermediate CNAME records at apex domains. This optimises multi-region failover latency, simplifies root-domain zone architecture, and improves routing performance within **Azure DNS**.

## Identity & Governance

- **Safe Key Rotation Metadata for Azure Cosmos DB** *(Generally Available)*\
  Administrative planes now expose granular last-used timestamp telemetry alongside master and secondary access keys. This visibility enables security operations teams to confidently plan, execute, and validate zero-downtime secret rotations while deprecating stale access keys across **Azure Cosmos DB**.
- **Choose Your Own Telephony (CYOT) Provider for Entra** *(Generally Available)*\
  Enterprises can now route multi-factor authentication SMS and voice verification traffic through existing, enterprise-contracted third-party telecommunications carriers. This expands carrier diversity, optimises regional messaging costs, and meets strict corporate regulatory agreements within **Microsoft Entra ID**.
- **Advanced Platform Metrics & Metrics Usage Insights** *(Generally Available)*\
  High-fidelity platform signals alongside granular workspace metric consumption telemetry are now accessible across central operational dashboards. This enables platform administrators to profile metric ingestion costs, detect unutilised monitoring sinks, and debug system trends with higher precision in **Azure Monitor**.

That’s a wrap on this weeks Azure updates, if you found this helpful make sure to follow [blog.atozazure.com](http://blog.atozazure.com) for future updates, guides, and technical insights.