---
title: "The A-Z Weekly Wrap: 2nd October 2026 (Late September – October 2026)"
seoTitle: "The A-Z Weekly Wrap: Azure Updates Oct 2026"
seoDescription: "This week's Azure platform news, covering AMD EPYC VM launches, key retirement dates, Azure Arc expansions, and instant VM restore points."
datePublished: 2026-10-02T19:38:13.809Z
cuid: cmurd8ec7000006nyhsoaak38
slug: weekly-wrap-20102026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/9db1d9a4-c0f4-4cbb-9ff8-aa95007a00c1.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/5a5b9e27-f957-4b39-b790-320f90a51ea2.jpg
tags: azure, updates, atozazure

---

Welcome to this week’s Microsoft Azure platform roundup. Keeping pace with cloud evolution is critical for maintaining performant, secure, and cost-effective environments. Below is a curated summary of key features, general availability milestones, previews, and service lifecycle notices announced over the past seven days to help you plan your architecture and engineering roadmaps.

## Compute & Containers

*   **Storage Optimized Lasv5 and Laosv5 Virtual Machine Series** *(Generally Available)*  
    Microsoft has launched the AMD EPYC (Turin)-powered Lasv5 and Laosv5 VM sizes, offering up to 160 vCPUs, 8 GiB of memory per core, and direct local NVMe capacity. This architectural addition provides high IOPS and high-throughput local disk storage suited for data-intensive transaction processing and indexing workloads in **Azure Virtual Machines**.
    
*   **Automatic Zone Placement for Virtual Machine Scale Sets** *(In Preview)*  
    A new intelligent orchestration feature dynamically assigns optimal availability zones for scale-out sets based on real-time datacentre capacity and SKU availability. This mitigates capacity constraint deployment failures and removes manual zone mapping overhead across **Azure Virtual Machine Scale Sets (VMSS)**.
    
*   **Azure Container Apps Express** *(Generally Available)*  
    The platform now provides a lightweight hosting tier featuring sub-second provisioning and automatic scale-to-zero capabilities without requiring upfront environment configuration. This streamlines containerised microservice deployments and minimises idle compute costs in **Azure Container Apps**.
    
*   **Ubuntu 26.04 LTS Node Pool Support** *(In Preview)*  
    Cluster operators can now deploy node pools based on the Ubuntu 26.04 Minimal OS image SKU. This reduces container host attack surfaces and operational footprint whilst aligning lifecycle roadmaps in **Azure Kubernetes Service (AKS)**.
    
*   **Retirement Notice: Dv3, Dsv3, Ev3, and Esv3 VM Series** *(Retiring)*  
    Microsoft has formally announced the end-of-life roadmap for legacy general-purpose and memory-optimised v3 virtual machines, setting a final retirement date of 15 November 2029. Engineering teams must schedule migration paths toward modern v5 or v6 hardware generations within **Azure Virtual Machines**.
    
*   **Retirement Notice: Azure Functions v1 Hosting on Azure Container Apps** *(Retiring)*  
    Support for the Functions v1 execution runtime hosted within containerised environments will cease on 29 September 2027. Teams running serverless code workloads must upgrade application code to modern runtime targets within **Azure Functions** and **Azure Container Apps**.
    
*   **Retirement Milestone: NVv3 and NVv4 GPU Virtual Machines** *(Retired)*  
    Effective 30 September 2026, the older generation Nvidia (NVv3) and AMD (NVv4) GPU virtual machines have reached final retirement in public regions. Unmigrated workloads running on these instances will be deallocated and must be transitioned to current NV-series SKUs in **Azure Virtual Machines**.
    

## AI & Tooling

*   **Azure Canvases for GitHub Copilot** *(Generally Available)*  
    Microsoft has introduced collaborative, interactive workspaces that embed live cloud telemetry, architectural dashboards, and deployment automation directly alongside developer conversations. This eliminates context-switching and enhances governance when inspecting environments via **GitHub Copilot in Azure**.
    

## Databases & Storage

*   **Managed SQL Performance Monitoring on Azure VMs** *(In Preview)*  
    A native, Microsoft-managed observability solution now captures and correlates diagnostic counters directly without requiring third-party monitoring agents or custom telemetry scripts. This accelerates database root-cause analysis and reduces operational overhead for **SQL Server on Azure Virtual Machines**.
    
*   **Azure Arc-Enabled SQL Server Regional Expansion** *(Generally Available)*  
    Centralised Azure governance, vulnerability assessment, automated patching, and hybrid license management have been extended to the Germany West Central and Italy North regions. This provides unified compliance and posture control for on-premises and edge databases integrated with **Azure Arc**.