---
title: "The A-Z Weekly Wrap: 2nd October 2026"
seoTitle: "The A-Z Weekly Wrap: Azure Updates Oct 2026"
seoDescription: "This week's Azure platform news, covering AMD EPYC VM launches, key retirement dates, Azure Arc expansions, and instant VM restore points."
datePublished: 2026-10-02T19:38:13.809Z
cuid: cmurd8ec7000006nyhsoaak38
slug: weekly-wrap-20102026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/9db1d9a4-c0f4-4cbb-9ff8-aa95007a00c1.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/5a5b9e27-f957-4b39-b790-320f90a51ea2.jpg
tags: azure, updates, atozazure

---

Welcome to this week’s atozazure weekly wrap for the 2nd October 2026. Below are all the key platform changes, additions and retirements for the past week.

## Compute & Containers

*   **Horizontal Scaling for Databricks Apps** *(Status: Generally Available)* You can now run Databricks apps across multiple instances behind a single unified URL with zero-downtime deployments and session affinity. This eliminates availability bottlenecks and significantly improves concurrency for production user-facing web apps running on **Azure Databricks**.
    
*   **Azure Virtual Desktop Classic Retirement** *(Status: Retiring)* Microsoft has officially sunsetted Azure Virtual Desktop (classic) as of the 30th September 2026 deadline, blocking inbound connections to classic management plane resources. Workloads must be fully transitioned to ARM-based host pools to restore connectivity and management capabilities on **Azure Virtual Desktop**.
    

## Databases & Analytics

*   **Lakeflow Jobs Table Update Triggers on OpenSharing & System Tables** *(Status: Generally Available)* Event-driven table update triggers can now monitor OpenSharing objects and system tables directly to kick off downstream ETL runs. This simplifies lakehouse pipelines and avoids costly scheduled polling mechanisms across shared datasets in **Azure Databricks**.
    
*   **Query Tags for Databricks SQL Warehouses** *(Status: Generally Available)* Workloads on serverless and classic SQL warehouses can now be tagged with custom key-value pairs that surface directly inside `system.query` telemetry. This introduces granular cost attribution and chargeback mapping for engineering teams utilising **Azure Databricks**.
    

## Networking & Security

*   **Inbound Private Link for Performance-Intensive Services** *(Status: Generally Available)* Azure Private Link integration is now generally available for high-throughput data paths, including Lakebase Autoscaling and Zerobus Ingest. This eliminates public data egress exposure while maintaining ultra-low latency enterprise network boundaries on **Azure Databricks**.
    
*   **Standalone Workload Sunsetting in Azure Communication Services** *(Status: Retiring)* Microsoft has announced the phased retirement of standalone calling and messaging endpoints in favour of Teams-aligned architectures (such as Teams Phone Extensibility). New sign-ups for retiring standalone features close on 23rd October 2026, requiring architects to align real-time communication stacks with Microsoft 365 services on **Azure Communication Services**.
    

## Governance & Management

*   **Unified Asset Tagging for Dashboards, Notebooks, and Genie Agents** *(Status: Generally Available)* Workspace assets, notebooks, and autonomous agents now support both governed Unity Catalog and ungoverned metadata key-value tags. This centralises compliance auditing, operational taxonomy, and access governance across **Azure Databricks**.
    
*   **Azure Developer CLI (azd) Extension Management & Concurrency Limits** *(Status: Generally Available)* The latest CLI update introduces versioned gRPC extension contracts, dependency-aware uninstalls, and per-phase concurrency throttling for package and deploy runs. This prevents deployment race conditions and standardises CI/CD pipeline automation for **Azure Developer CLI**.
    

* * *

That’s a wrap on this week's Azure platform changes. I hope this quick overview helps streamline your upcoming engineering sprints. If you found it helpful, make sure to follow for future updates.