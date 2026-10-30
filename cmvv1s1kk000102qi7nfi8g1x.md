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

Welcome to this week’s atozazure weekly wrap for the 30th October 2026. Below are all the key platform changes, additions and retirements for the past week.

## Storage & Databases

- **Azure Backup: Item-Level Recovery for Premium SSD v2 and Ultra Disks** *(Generally Available)*\
  Azure Backup now enables Item-Level Recovery (ILR) for virtual machines running on Premium SSD v2 and Ultra Disks supporting both 512-byte and 4KB logical sector sizes. This capability significantly improves recovery point objectives (RPO) and operational agility by allowing granular file and folder extraction without requiring full volume or virtual machine restores in **Azure Backup**.
- **Azure Data Lake Storage: ABFS Vectored Read** *(Generally Available)*\
  The Azure Blob File System (ABFS) driver now supports Vectored Read APIs, coalescing disjointed columnar file segments into unified asynchronous read requests. This architectural enhancement cuts round-trip request overhead and latency significantly for analytics engines querying Parquet and ORC formats hosted on **Azure Data Lake Storage**.
- **Azure Cosmos DB: Safe Key Rotation** *(Generally Available)*\
  Safe Key Rotation introduces automated pre-flight validation against account key access logs, blocking key regeneration if active transactions occurred within the preceding 12 hours. This eliminates accidental production outages caused by premature credential revocation during secrets lifecycle transitions or migration to Microsoft Entra ID in **Azure Cosmos DB**.

## Identity & Access Management

- **Microsoft Entra ID: Choose Your Own Telephony (CYOT)** *(In Preview)*\
  Organizations can now integrate approved third-party telecommunications providers to deliver SMS and voice multi-factor authentication (MFA) verifications directly. This provides enhanced compliance and cost control over telephony routes, bypassing standard platform SMS delivery rails for **Microsoft Entra ID**.
- **Entra Global Secure Access Client for Windows v2.34.222** *(Generally Available)*\
  The latest Windows client update adds refined local network bypass rules, granular Conditional Access evaluation points, and expanded client-side connection telemetry. These enhancements reduce network path friction for split-tunnel scenarios and accelerate diagnostics in **Microsoft Entra Private Access** and **Microsoft Entra Internet Access**.

## Networking & Infrastructure

- **Disable Virtual Network Peering Route** *(In Preview)*\
  A new control flag in user-defined route tables allows platform engineers to selectively suppress system-generated peering routes across interconnected virtual networks. This enables strict hub-spoke traffic enforcement and prevents inadvertent transitive routing without requiring complex subnet-level route overriding in **Azure Virtual Network**.
- **Azure Application Gateway: Keyless TLS with Managed HSM** *(Generally Available)*\
  Application Gateway v2 now terminates TLS handshakes by offloading cryptographic signature operations directly to Azure Key Vault Managed HSM via remote procedure calls. Private certificate keys never leave the FIPS 140-3 Level 3 hardware boundary, satisfying stringent regulatory requirements for public sector and financial workloads using **Azure Application Gateway**.
- **Azure Front Door Premium: Service Tag Match Conditions in WAF** *(Generally Available)*\
  Azure Web Application Firewall (WAF) custom rule policies now natively support service tags as matching criteria. This simplifies ingress filtering by dynamically aligning WAF rule execution with Microsoft-maintained IP address prefixes for downstream services behind **Azure Front Door**.
- **Azure DNS: Traffic Manager Linked Records** *(Generally Available)*\
  Apex and subdomain DNS record sets can now be linked directly to Azure Traffic Manager profiles without intermediary CNAME or alias flattening workarounds. This native integration reduces resolution hops and optimizes global routing resilience within **Azure DNS**.

That’s a wrap on this weeks Azure updates, if you found this helpful make sure to follow [blog.atozazure.com](http://blog.atozazure.com) for future updates, guides, and technical insights.