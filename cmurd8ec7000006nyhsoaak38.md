---
title: "The A-Z Weekly Wrap: 2nd October 2026 (Late September – October 2026)"
seoTitle: "The A-Z Weekly Wrap: Azure Updates Oct 2026"
seoDescription: "This week's Azure platform news, covering AMD EPYC VM launches, key retirement dates, Azure Arc expansions, and instant VM restore points."
datePublished: 2026-10-02T19:38:13.809Z
cuid: cmurd8ec7000006nyhsoaak38
slug: weekly-wrap-20102026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/9db1d9a4-c0f4-4cbb-9ff8-aa95007a00c1.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/44d286af-fc3a-4a10-963d-669a4fd16638.jpg
tags: azure, updates, atozazure

---

## Compute & Containers

* **Storage-Optimised Lasv5 and Laosv5 VM Series** *(Generally Available)*  
  Powered by 5th Gen AMD EPYC™ processors (Turin), these newly launched virtual machine sizes offer up to 160 vCPUs, 8 GiB RAM per core, and 720 GB of local NVMe disk capacity per vCPU. They deliver substantial throughput and low-latency disk IOPS for dense databases, data warehouses, and large-scale big data workloads on **Azure Virtual Machines**.

* **Automatic Zone Placement for Virtual Machine Scale Sets** *(In Preview)*  
  Azure can now dynamically balance and place VM instances across optimal Availability Zones based on real-time datacentre capacity, SKU health, and resource distribution. This simplifies high-availability deployments by removing the overhead of hardcoding or manually managing zone distribution across **Azure Virtual Machine Scale Sets (VMSS)**.

* **Ubuntu 26.04 LTS Worker Node Pools** *(In Preview)*  
  Cluster operators can now deploy `Ubuntu2604` minimal OS images for node pools in **Azure Kubernetes Service (AKS)**. The streamlined base image reduces container footprint, accelerates node provisioning and scale-out times, and significantly reduces the host attack surface.

* **Retirement: Functions v1 Hosting on Azure Container Apps** *(Retiring)*  
  Microsoft has set a retirement milestone of 29 September 2027 for the legacy v1 hosting model of Azure Functions within **Azure Container Apps**. Teams running legacy microservice architectures should plan migrations toward modern containerised runtimes to ensure ongoing support.

* **Retirement: Dv3, Dsv3, Ev3, and Esv3 VM Families** *(Retiring)*  
  The ubiquitous v3 general-purpose and memory-optimised instances have entered their formal decommissioning schedule ahead of their 15 November 2029 sunset date. Operators should evaluate newer AMD (v5/v6) or Intel iterations to achieve better price-performance across their **Azure Virtual Machines** estate.

* **Decommissioned: NVv3 and NVv4 GPU Workstations** *(Retired)*  
  Effective 30 September 2026, the older NVIDIA (NVv3) and AMD Radeon Instinct (NVv4) virtual workstation SKUs have reached full end-of-life status. Workloads must transition to current NV-series alternatives on **Azure Virtual Machines**.

---

## AI & Platform Tooling

* **Azure Canvases for GitHub Copilot** *(Generally Available)*  
  Engineering teams can now take advantage of interactive, contextual visual canvases within Copilot chat. This feature integrates infrastructure telemetry, cost exploration, and direct provisioning guidance natively inside developer workflows across **GitHub Copilot and Azure Developer Tools**.

---

## Databases & Hybrid Infrastructure

* **Built-in Performance Monitoring for SQL Server on Azure VMs** *(In Preview)*  
  Managed query telemetry and diagnostic tracking are now available natively without requiring custom maintenance scripts or third-party agent installations, providing streamlined operational observability for **SQL Server on Azure Virtual Machines**.

* **Flexible Compute-to-Memory Allocation for SQL Managed Instance** *(Generally Available)*  
  Database administrators can now dynamically modify memory ratios without undergoing costly tier migrations. This enables granular tuning for high-cache, memory-intensive transactional workloads hosted on **Azure SQL Managed Instance**.

* **Azure Arc-Enabled SQL Server Expansion** *(Generally Available)*  
  Governance, automated security patching, licensing optimisation, and compliance posture assessments through **Azure Arc** are now locally available in the Germany West Central and Italy North cloud regions for hybrid and multi-cloud database estates.

---

## Governance, Continuity & Edge Infrastructure

* **Instant Access for VM Restore Points** *(Generally Available)*  
  Disaster recovery runbooks receive a major boost with instantaneous disk recovery from application-consistent snapshots for Premium SSD v2 and Ultra Disk configurations, dramatically reducing Recovery Time Objectives (RTO) via **Azure Backup**.

* **Luxembourg Extended Zone** *(Generally Available)*  
  Organizations requiring ultra-low-latency processing or strict local data residency can now deploy compute and storage resources at the new Luxembourg edge site connected back to core European regions through **Azure Extended Zones**.

---

*Did any of these updates affect your current architecture or migration roadmap? Let us know your thoughts or implementation questions in the comments below.*