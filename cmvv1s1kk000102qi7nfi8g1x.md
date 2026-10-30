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

## Networking & Security

- **Azure DNS Integration with Traffic Manager Linked Records** *(Generally Available)*\
  Direct linked record support between **Azure DNS** and **Azure Traffic Manager** profiles eliminates intermediate CNAME resolution hops, streamlining geo-routing management and reducing client-side DNS lookup latency.
- **Keyless TLS via Azure Key Vault Managed HSM for Application Gateway** *(Generally Available)*\
  **Application Gateway v2** now natively offloads TLS handshakes to **Azure Key Vault Managed HSM** without private keys ever leaving hardware cryptographic boundaries, reinforcing FIPS 140-2 Level 3 cryptographic compliance.
- **External Key Management for Azure Key Vault Managed HSM** *(Generally Available)*\
  Sovereign key orchestration allows enterprise workloads to control root encryption keys external to Azure within **Azure Key Vault Managed HSM**, preserving strict physical cryptographic isolation for cross-region data estates.
- **Standard Service Endpoints for PaaS Integration** *(Generally Available)*\
  Enhanced **Azure Virtual Network** service endpoints scale perimeter security boundary controls across core PaaS tiers, reducing subnet scaling constraints whilst enforcing strict network isolation.
- **Hardware Audit Logging for Azure Cloud HSM** *(Generally Available)*\
  Tenant instances under **Azure Dedicated HSM / Cloud HSM** now output tamper-evident hardware-level audit trails, accelerating compliance verification and forensic reporting for strictly regulated environments.

## Compute & Containers

- **Automatic Zone Balance for Virtual Machine Scale Sets** *(Generally Available)*\
  Continuous topology telemetry in **Azure Virtual Machine Scale Sets (VMSS)** automatically redistributes VM instances across Availability Zones during capacity drift, ensuring uninterrupted SLA availability without operational intervention.
- **Emergency Security Runtime Rollouts for Azure App Service** *(Generally Available)*\
  Platform-wide runtime patch updates for PHP, Node.js, and Python alongside intermediate CA trust updates have been deployed across **Azure App Service**, addressing critical remote execution vulnerabilities and certificate trust paths.

## Databases, Storage & Analytics

- **Private Network Gateway for Azure Databricks** *(In Preview)*\
  Serverless compute environments in **Azure Databricks** can now route outbound connectivity to private virtual networks and on-premises hubs via a managed private egress gateway, removing complex NAT gateway configurations.
- **Cross-Region Data Copy and Synchronisation via Azure Storage Mover** *(In Preview)*\
  Orchestrated delta replication across storage accounts and regions is now supported in **Azure Storage Mover**, enabling automated hybrid and cloud-to-cloud disaster recovery pipelines for **Azure Files**.
- **Item-Level Recovery for Premium SSD v2 and Ultra Disks** *(Generally Available)*\
  Granular file- and folder-level restore capabilities in **Azure Backup** now support next-generation high-performance **Azure Managed Disks (Premium SSD v2 & Ultra Disk)**, cutting Recovery Time Objectives (RTO) for I/O-intensive workloads.
- **Safe Key Rotation Visibility for Azure Cosmos DB** *(Generally Available)*\
  Enhanced lifecycle telemetry in **Azure Cosmos DB** provides proactive audit visibility into primary and secondary key rotation workflows, mitigating client credential drops and inadvertent access disruptions.

## AI & Machine Learning

- **Decisions API Availability in Microsoft Azure AI Foundry** *(Generally Available)*\
  The OpenAI Decisions API is integrated directly into **Azure AI Foundry**, offering low-latency structured decision-tree evaluations and reasoning controls for enterprise agentic architectures.
- **Per-Agent Managed Identity Support in Microsoft Copilot Studio** *(Generally Available)*\
  Autonomous agents built in **Microsoft Copilot Studio** can now be assigned granular **Microsoft Entra ID** managed identities, enforcing least-privilege role assignments across backing Azure enterprise APIs and vector stores.

## Retirements & Lifecycle Notices

- **Azure Functions .NET In-Process Model Retirement Reminder** *(Retiring)*\
  Formal support for the .NET in-process execution model in **Azure Functions** concludes on 10 November 2026; development teams must transition existing Function Apps to the out-of-process isolated worker model to maintain platform support.
- **Azure Key Vault Legacy Control Plane API Versions Deprecation Notice** *(Retiring)*\
  Management API versions prior to `2026-02-01` for **Azure Key Vault** will cease functioning on 27 February 2027, requiring platform engineers to upgrade deployment scripts and toolsets to Azure CLI 2.90.0+ or Az.KeyVault 6.6.1+.

That’s a wrap on this weeks Azure updates, if you found this helpful make sure to follow [blog.atozazure.com](http://blog.atozazure.com) for future updates, guides, and technical insights.