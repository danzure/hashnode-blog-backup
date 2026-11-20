---
title: "The A-Z Weekly Wrap: 20th November, 2026 (Microsoft Ignite Special 2026)"
seoTitle: "The A-Z Weekly Wrap: Azure Updates 20th Nov 2026"
seoDescription: "Latest Azure platform updates for the 20th November 2026, covering key announcements from Microsoft Ignite "
datePublished: 2026-11-20T15:48:35.834Z
cuid: cmwp5ltwd000008l886i1hwbg
slug: weekly-wrap-20112026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/5852f1bf-0315-40d8-bcda-fa9725d47e90.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/4515c087-f9fb-40a5-ae96-4a8272c20276.jpg
tags: ai, microsoft, azure, databases, devops, containers, compute, copilot, agentic-ai

---

Welcome to this week’s atozazure weekly wrap Microsoft Ignite Special for the 20th November 2026. Below are all the key platform changes, additions and retirements for the past week.

## AI & Machine Learning

- **External Agents Support in Microsoft Foundry** *(Generally Available)*\
  External agents running outside **Microsoft Foundry** that send OpenTelemetry traces to Application Insights can now be registered directly in Foundry to observe and evaluate behaviour without migrating or rebuilding workloads.
- **MAI Code 2 and MAI Code 2 Flash Models** *(Generally Available)*\
  Microsoft introduced its second-generation in-house agentic coding models in **Microsoft Foundry** and GitHub Copilot, supporting a 1.05 million token context window and five reasoning levels for multi-file implementation, debugging, and rapid code iteration.
- **Microsoft Foundry on Azure Kubernetes Service (AKS)** *(In Preview)*\
  New preview capabilities extend **Microsoft Foundry** to **Azure Kubernetes Service (AKS)** via AKS AI Manager, allowing teams to deploy open-weight models and Foundry-hosted agents onto existing customer-managed clusters.
- **Microsoft Foundry Support for Business Applications in Work IQ** *(Generally Available)*\
  Developers can now connect agents in **Microsoft Foundry** to enterprise systems such as Dynamics 365 and Salesforce via **Work IQ**, reducing custom integration overhead and turning business data into actionable workflows.
- **Microsoft-Decision-1.1 Model** *(Generally Available)*\
  The multimodal **Microsoft-Decision-1.1** model is now generally available in **Microsoft Foundry**, delivering low-latency routing, data labelling, personalisation, and content filtering for enterprise deployments.
- **Model Router Enhancements in Microsoft Foundry** *(Generally Available)*\
  **Microsoft Foundry** Model Router adds Auto and Auto Advanced modes alongside workload-level cost and quality evaluation to dynamically steer requests across frontier and open models.
- **New Azure Databricks Environment on Azure Government** *(In Preview)*\
  A new **Azure Databricks** beta environment is now available on Microsoft Azure Government, bringing modern data engineering and AI capabilities to government cloud workloads.
- **Voice Agents in Microsoft Foundry Agent Service** *(Generally Available)*\
  **Microsoft Foundry** Agent Service now supports production voice agents with low-latency, multilingual speech capabilities for real-time conversational customer experiences.

## Compute & Containers

- **Agent Sandbox Cluster Extension for AKS** *(In Preview)*\
  The Agent Sandbox extension for **Azure Kubernetes Service (AKS)** enables teams to execute agent-generated code inside isolated, virtual-machine-level sandboxes.
- **Azure App Service Builder** *(In Preview)*\
  **Azure App Service** Builder provides a guided experience to accelerate moving application code into running, managed web applications.
- **Azure Chaos Studio Workspaces and AKS Extension** *(Generally Available)*\
  **Azure Chaos Studio** introduces reusable disruption workspaces and a native **Azure Kubernetes Service (AKS)** extension to simulate availability-zone loss, database failovers, and pod faults with reduced permissions.
- **Azure Cobalt 200 Virtual Machines** *(Generally Available)*\
  Next-generation Arm-based **Azure Virtual Machines** (Dpsv7, Dplsv7, Epsv7, Mpsv4, and Lpsv5 series) powered by custom Cobalt 200 silicon deliver up to 50% higher CPU performance than Cobalt 100 alongside boost modes and up to 23 TB of local storage.
- **Azure Compute Spot Plus** *(In Preview)*\
  Spot Plus introduces a new tier for **Azure Spot Virtual Machines** targeting at least 60 minutes of uninterrupted runtime on a best-effort basis, waiving compute charges if eviction occurs within the first hour.
- **Azure Ebsv6 and Ebdsv6 Virtual Machines** *(Generally Available)*\
  Powered by 5th Gen Intel Xeon processors and Azure Boost, the memory-optimised Ebsv6 and Ebdsv6 **Azure Virtual Machines** deliver higher remote storage throughput and IOPS for data-intensive workloads.
- **Azure Linux 4.0** *(Generally Available)*\
  **Azure Linux** 4.0 is now generally available as the latest Microsoft-maintained container host OS release for AKS and cloud-native workloads.
- **Compute Templates for Azure Virtual Machines** *(In Preview)*\
  Limited preview support for compute templates simplifies **Azure Virtual Machines** configuration management by enabling teams to define, version, and reuse standardised VM specifications.
- **Confidential VMs with Intel TDX Support on AKS** *(Generally Available)*\
  **Azure Kubernetes Service (AKS)** now supports Confidential Virtual Machines backed by Intel Trust Domain Extensions (TDX) to isolate sensitive container workloads in hardware-encrypted memory.
- **Flex Nodes for AKS** *(In Preview)*\
  Flex nodes extend **Azure Kubernetes Service (AKS)** clusters to customer-managed servers outside Azure, providing unified Kubernetes orchestration across hybrid environments.
- **OS-Level Dependency Support via Containers for Azure Functions Flex Consumption** *(In Preview)*\
  Developers using **Azure Functions** Flex Consumption plans can now package custom OS-level dependencies via container images while retaining serverless scaling.
- **Task Queues for Azure Functions Durable Task Scheduler** *(In Preview)*\
  Task Queues in **Azure Functions** provide managed work distribution and routing for durable task orchestrations.
- **VM Adaptive Placement** *(In Preview)*\
  VM adaptive placement improves **Azure Virtual Machines** deployment success rates during regional capacity constraints by dynamically selecting optimal underlying infrastructure.
- **Windows Trusted Launch on AKS** *(In Preview)*\
  **Azure Kubernetes Service (AKS)** adds Trusted Launch support in public preview for Windows node pools, providing verified boot-chain protection for regulated workloads.

## Databases & Storage

- **AI Model Management in Azure HorizonDB** *(In Preview)*\
  Limited preview support in **Azure HorizonDB** simplifies registering, invoking, and managing AI models directly within the PostgreSQL-compatible database engine.
- **AI-Assisted Data Modeler in Azure Cosmos DB Extension for VS Code** *(In Preview)*\
  Updates to the Visual Studio Code extension for **Azure Cosmos DB** introduce an AI-assisted data modeller, account insights, and guided schema recommendations.
- **Azure Backup for Azure Cosmos DB** *(Generally Available)*\
  Vaulted backup support in **Azure Backup** provides an independent, immutable, long-term data protection layer with centralised retention policies for **Azure Cosmos DB** accounts.
- **Azure Cosmos DB SDK for Rust** *(Generally Available)*\
  A native Rust SDK for **Azure Cosmos DB** is now generally available for building high-performance, memory-safe cloud applications.
- **Azure Cosmos DB Shell** *(Generally Available)*\
  The new command-line **Azure Cosmos DB** Shell enables developers and AI agents to query, inspect, and manage database resources interactively.
- **Azure HorizonDB** *(Generally Available)*\
  **Azure HorizonDB**, a fully managed PostgreSQL-compatible database service with built-in vector indexing and millisecond latency for transactional and AI workloads, is now generally available.
- **Azure SQL Database Local Container** *(In Preview)*\
  Developers can now run the **Azure SQL Database** engine locally in a container—complete with vector search, ledger, and secure enclave capabilities—without an Azure subscription.
- **Cobalt 200 Compute and Diskless Tier for Azure Database for PostgreSQL** *(Generally Available)*\
  **Azure Database for PostgreSQL** flexible server now supports Arm-based Cobalt 200 compute alongside Intel and AMD v5 diskless tiers for improved price-performance.
- **Cross-Subscription Backup for Azure Virtual Machines in Azure Backup** *(Generally Available)*\
  **Azure Backup** now allows organisations to protect **Azure Virtual Machines** using a Recovery Services vault located in a separate Azure subscription.
- **Database Agent for SQL with Contextual Copilot** *(In Preview)*\
  Database Agent provides AI-generated, evidence-grounded diagnostics and remediation recommendations for detected issues across **Azure SQL Database** and **Azure SQL Managed Instance**.
- **Database Hub Real-Time Performance Dashboards** *(Generally Available)*\
  Database Hub in Microsoft Fabric delivers unified, real-time performance monitoring dashboards across **Azure SQL**, **Azure Database for PostgreSQL** flexible server, and **Azure Cosmos DB**.
- **DocumentDB Enabled by Azure Arc and Azure Local** *(In Preview)*\
  New preview offerings extend **Azure DocumentDB** to hybrid, multicloud, and **Azure Local** environments for MongoDB-compatible workloads with data sovereignty requirements.
- **Fine-Grained Role-Based Access Control in Azure DocumentDB** *(In Preview)*\
  **Azure DocumentDB** now supports scoping custom RBAC roles and least-privilege permissions down to individual databases and collections.
- **Immutable Snapshots for Azure Disk Storage** *(In Preview)*\
  **Azure Disk Storage** introduces read-only, immutable snapshots to protect backups against ransomware and accidental or malicious deletion.
- **Managed MCP Server and Embedding Generation in Azure Cosmos DB** *(In Preview)*\
  **Azure Cosmos DB** previews a managed Model Context Protocol (MCP) server and built-in embedding generation to streamline agentic retrieval workflows.
- **Migrate PostgreSQL Servers to Azure HorizonDB** *(In Preview)*\
  **Azure Database Migration Service** adds public preview support for migrating existing PostgreSQL instances directly to **Azure HorizonDB**.
- **Redis 8 Preview and Agent Kit in Azure Managed Redis** *(In Preview)*\
  **Azure Managed Redis** introduces a preview of Redis 8 alongside an agent kit that guides AI-assisted development tools on optimal connection and caching patterns.
- **Semantic Reranker and Full-Text Relevance Scores in Azure Cosmos DB** *(Generally Available)*\
  **Azure Cosmos DB** adds general availability for semantic reranking and full-text relevance scoring to improve hybrid search accuracy.
- **Snapshot Backup for SQL Server in Azure VMs** *(Generally Available)*\
  **Azure Backup** now supports fast, snapshot-based backups for **SQL Server on Azure Virtual Machines**.
- **Throughput Buckets in Azure Cosmos DB** *(Generally Available)*\
  Throughput buckets in **Azure Cosmos DB** allow workloads to allocate and isolate Request Units (RUs) across priority tiers to prevent noisy-neighbour throttling.

## Governance, Management & Developer Tools

- **Agent 365 Cost Management** *(In Preview)*\
  Microsoft Agent 365 introduces centralised FinOps visibility, usage tracking, spending limits, and proactive alerts for usage-based AI agents and Copilot services.
- **Azure AI Gateway** *(Generally Available)*\
  Previously offered as a tier within **Azure API Management**, **Azure AI Gateway** is now generally available as a dedicated managed service for governing, routing, and securing AI model and agent endpoints.
- **Azure Catalyst and Azure Catalyst Agent** *(Generally Available)*\
  **Azure Catalyst** unifies application discovery, dependency mapping, and agent-led modernisation across Azure Copilot and GitHub Copilot, with preview support for BizTalk-to-Logic Apps migrations and cost comparisons.
- **Azure Copilot Deployment Agent** *(Generally Available)*\
  The **Azure Copilot** deployment agent converts natural-language architectural requirements directly into deployed Azure infrastructure workloads.
- **Azure Infrastructure Resiliency Manager** *(Generally Available)*\
  **Azure Infrastructure Resiliency Manager** provides a unified, goal-driven control plane for assessing, configuring, and validating resiliency across Azure workloads.
- **Azure Monitor Health Models** *(Generally Available)*\
  **Azure Monitor** health models map live telemetry to application architecture and business priorities, giving operators and AI agents structured context for faster root-cause remediation.
- **Azure Monitor Traces and Trace Analytics** *(In Preview)*\
  New distributed tracing analytics in **Azure Monitor** enable engineers to query, compare, and isolate high-volume agent and microservice traces.
- **Azure SRE Agent Operations in Azure Container Apps and Microsoft Teams** *(In Preview)*\
  **Azure SRE Agent** adds interactive debugging inside the **Azure Container Apps** portal alongside Microsoft Teams integration and Microsoft Entra Agent ID governance.
- **Azure Workload Center for SAP and Oracle** *(In Preview)*\
  Limited preview support in **Azure Workload Center** extends agentic monitoring and operational workflows to enterprise SAP and Oracle estates.
- **Decision Actions and Virtual Network Integration in Azure Logic Apps Automation** *(In Preview)*\
  **Azure Logic Apps** adds public preview support for AI-powered decision actions, private VNet integration, MLLP/MSMQ connectors, and a unified monitoring dashboard, alongside general availability for the HL7 connector and Managed Connectors in Azure Functions.
- **Sovereign Control Panel and Data Guardian Integration** *(In Preview)*\
  The Microsoft Sovereign Cloud **Sovereign Control Panel** enters public preview with integrated discovery for generally available Data Guardian capabilities to manage sovereign compliance controls.

## Networking & Security

- **Agent Grid Zero Trust Networking** *(In Preview)*\
  **Agent Grid** brings identity-based Zero Trust network isolation and policy enforcement to AI agent communications across supported Azure environments.
- **Azure Application Gateway Confidential Compute Support** *(In Preview)*\
  **Azure Application Gateway** adds confidential computing support to protect sensitive traffic payloads in memory while requests are actively processed.
- **Azure Bastion RDP and SSH Vision** *(In Preview)*\
  **Azure Bastion** Premium introduces AI-assisted session review that summarises recorded RDP and SSH administrative sessions, highlights risky actions, and generates full SSH command logs.
- **Azure DDoS Protection Custom Policy** *(Generally Available)*\
  **Azure DDoS Protection** custom policies allow network teams to configure granular, protocol-specific mitigation thresholds tailored to application traffic profiles.
- **Azure Network Watcher AI Connection Troubleshoot Summaries and Rule Recommendations** *(In Preview)*\
  **Azure Network Watcher** introduces AI-generated summaries for connection troubleshoot diagnostics, automated NSG rule recommendations, and live resource health overlays within Connection Monitor topologies.
- **JWT Validation with Azure Front Door Auth Policy** *(In Preview)*\
  **Azure Front Door** Auth Policy adds native JSON Web Token (JWT) validation at the network edge before requests reach backend origins.
- **Microsoft Entra Agent ID for Local Devices and Intune Agent Controls** *(In Preview)*\
  **Microsoft Entra** extends Agent ID to locally running device agents while Microsoft Intune adds policy controls to block unapproved agents from accessing corporate data.
- **Project Nova Cryptographic Verification** *(In Development)*\
  Project Nova enters private preview, enabling regulated organisations to independently verify specific data claims without exposing underlying confidential datasets.
- **Rate Limit Grouping for Azure Front Door Premium WAF** *(In Preview)*\
  **Azure Front Door** Premium Web Application Firewall (WAF) adds rate limit grouping to aggregate and throttle incoming request rates across custom attribute keys.

That’s a wrap on this weeks Azure updates, if you found this helpful make sure to follow [blog.atozazure.com](http://blog.atozazure.com) for future updates, guides, and technical insights.