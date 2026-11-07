---
title: "The A-Z Weekly Wrap: 6th November 2026"
seoTitle: "Azure Weekly Wrap: 06th Nov 2026"
seoDescription: "Latest Azure platform updates for the 6th November 2026, covering key announcements across networking, security, compute, databases, and AI"
datePublished: 2026-11-06T14:07:29.182Z
cuid: cmw51tvif000102ml3ay25bjl
slug: weekly-wrap-06112026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/4af3d744-4251-4641-bb0b-7032a52560e9.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/26760c59-6386-490d-826b-3f2c2f24c30e.jpg
tags: ai, microsoft, azure, devops, containers, ml, azure-devops, atozazure

---

Welcome to this week’s atozazure weekly wrap for the 6th November 2026. Below are all the key platform changes, additions and retirements for the past week.

## Compute & Containers

- **Multi-disk crash-consistent VM restore points for Premium SSD v2 and Ultra Disks** *(In Preview)*\
  Extends multi-disk crash-consistent restore point capabilities to Premium SSD v2 and Ultra data disks attached to SCSI-based **Azure Virtual Machines**, enabling write-order-consistent snapshots and rapid Instant Access recovery without requiring guest agent quiescing.
- **Enhanced Azure Site Recovery support for VMSS Flex** *(Generally Available)*\
  Improves target configuration and end-to-end disaster recovery workflows—including failover, reprotection, and failback—for **Azure Virtual Machine Scale Sets** (Flexible orchestration) replicating across **Azure Site Recovery**.
- **Azure Site Recovery for Azure Local** *(Generally Available)*\
  Delivers production-ready, portal-driven hypervisor replication and automated VM failover from **Azure Local** clusters to Azure, adding full compatibility for hosts enforcing Windows Defender Application Control (WDAC).
- **Large OS Disk Encryption for Azure Confidential VM migrations** *(Generally Available)*\
  Enables workloads with large OS disks to migrate directly into **Azure Confidential Virtual Machines** with full disk encryption enabled, strengthening data-in-use protection and compliance during lift-and-shift modernisation.

## AI & Machine Learning

- **Microsoft Foundry extension for Azure Developer CLI (v1.0)** *(Generally Available)*\
  Releases version 1.0 of the `microsoft.foundry` extension bundle for **Azure Developer CLI** (`azd`), providing a production-supported command-line workflow to scaffold, test, and deploy enterprise AI agents in **Microsoft Foundry**.
- **Updated retirement dates for GPT-4o and GPT-5.1 models** *(Retiring)*\
  Revises the scheduled model deprecation timelines for `gpt-4o` and `gpt-5.1` deployments within **Microsoft Foundry**, giving engineering teams adjusted migration windows to transition active inference workloads to newer foundational models.

## Networking & Security

- **WAF Insights for Azure Application Gateway** *(Generally Available)*\
  Integrates interactive **Azure Monitor** workbooks directly into **Azure Web Application Firewall** on **Azure Application Gateway**, combining Log Analytics diagnostic queries and near-real-time metrics to streamline attack triage, false-positive tuning, and rule correlation.
- **Application rules for IPv6 on Azure Firewall** *(In Preview)*\
  Adds FQDN filtering and outbound HTTP/S and MSSQL application rule enforcement for IPv6 traffic on dual-stack **Azure Firewall** deployments, achieving policy parity across IPv4 and IPv6 network topologies.
- **HTTP DDoS ruleset for Azure Front Door Premium WAF** *(Generally Available)*\
  Provides managed Layer 7 HTTP flood mitigation rules within **Azure Web Application Firewall** on **Azure Front Door** Premium, automatically detecting and throttling volumetric application-layer traffic anomalies at the global edge.
- **Private ingress, JWT validation, and MCP gateway for Application Gateway for Containers** *(In Preview)*\
  Introduces private network ingress exposure, native JSON Web Token (JWT) pre-authentication at the proxy layer, and Model Context Protocol (MCP) gateway routing capabilities for **Application Gateway for Containers**.
- **Route maps for Azure Route Server** *(Generally Available)*\
  Enables granular BGP attribute manipulation, prefix filtering, and route steering policies directly on **Azure Route Server**, simplifying complex multi-cloud and SD-WAN network virtual appliance (NVA) integrations.

## Databases & Storage

- **Azure Database for PostgreSQL stable REST API version 2026-10-01** *(Generally Available)*\
  Releases the `2026-10-01` stable Resource Manager control-plane API for **Azure Database for PostgreSQL** Flexible Server, bringing GA support to programmatic FIPS configuration, immutable backup provisioning, pre-upgrade validation checks, and scheduled maintenance management.
- **Lockable point-in-time restore (PITR) backup immutability for Azure SQL** *(In Preview)*\
  Allows administrators to permanently lock point-in-time restore backup retention windows up to 35 days across **Azure SQL Database** and **Azure SQL Managed Instance**, preventing premature backup deletion or retention reduction in regulated environments.
- **Storage Actions task propagation and execution controls** *(Generally Available)*\
  Enhances serverless storage management in **Azure Storage Actions** with automated task definition propagation across target accounts, refined execution controls, and case-sensitive condition matching.
- **Capacity details report in Azure Storage Discovery** *(In Preview)*\
  Adds granular metadata aggregation across storage accounts, containers, and prefixes in **Azure Blob Storage**, giving platform and FinOps teams visibility into object size distribution, data age, and tiering efficiency via **Azure Storage Discovery**.
- **Change from virtual network integration to private endpoint networking in Azure Database for PostgreSQL** *(Generally Available)*\
  Supports in-place network architecture migration from delegated subnet VNet injection to Private Link private endpoints and public firewall access on **Azure Database for PostgreSQL** Flexible Server without requiring a full database dump and restore.

## Governance, Management & Developer Tools

- **Extended retirement deadline for Application Insights query API keys** *(Retiring)*\
  Extends the deprecation deadline for legacy query API keys in **Azure Monitor Application Insights** until 31 March 2027, providing additional time for teams to migrate programmatic telemetry queries to **Microsoft Entra ID** authentication.
- **On-premises NAS share discovery and assessment in Azure Migrate** *(In Preview)*\
  Expands discovery and migration readiness assessments in **Azure Migrate** to cover enterprise Network Attached Storage (NAS) shares, including Dell PowerScale and NetApp ONTAP estates, streamlining file workload migration planning.
- **Streamlined private offer setup in Microsoft Marketplace** *(Generally Available)*\
  Introduces flexible pricing terms and simplified commercial configuration workflows for private offers in **Azure Marketplace**, accelerating enterprise software procurement and cloud spend alignment.

That’s a wrap on this weeks Azure updates, if you found this helpful make sure to follow [blog.atozazure.com](http://blog.atozazure.com) for future updates, guides, and technical insights.