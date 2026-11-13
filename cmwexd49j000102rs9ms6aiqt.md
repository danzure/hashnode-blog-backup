---
title: "The A-Z Weekly Wrap: 13th November 2026"
seoTitle: "The A-Z Weekly Wrap: Azure Updates 13th Nov 2026"
seoDescription: "Latest Azure platform updates for the 13th November 2026, covering key announcements across AI, Compute, and Networking"
datePublished: 2026-11-13T12:00:00.000Z
cuid: cmwexd49j000102rs9ms6aiqt
slug: weekly-wrap-13112026
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/ede4e69f-5bb7-485d-adde-86d8248b5f33.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/8eee47c7-0588-4f14-9b4a-9923a5e860e5.jpg
tags: ai, microsoft, azure, database, networking, containers, atozazure

---

Welcome to this week’s atozazure weekly wrap for the 13th November 2026. Below are all the key platform changes, additions and retirements for the past week.

## AI & Machine Learning

- **Claude Fable 5.2 and Mythos 5.2 in Microsoft Foundry** *(Generally Available)*\
  Anthropic’s Claude Fable 5.2 and Fable 5.2 Fast models are now generally available in **Microsoft Foundry** for complex software engineering, quantitative finance, and scientific workflows. Claude Mythos 5.2 is also introduced for authorised organisations requiring specialised capabilities in cybersecurity and life sciences.
- **Durable Task extension for Microsoft Agent Framework** *(Generally Available)*\
  The Durable Task extension for **Microsoft Agent Framework** is now generally available for .NET and Python, enabling stateful, fault-tolerant multi-agent orchestrations. It automatically checkpoints execution history and replays saved results across **Azure Functions** or self-hosted environments without incurring duplicate token or inference costs during recovery.
- **Kimi K3.1 Pro via Fireworks in Microsoft Foundry** *(Generally Available)*\
  Moonshot AI’s open-weight multimodal Kimi K3.1 Pro model is now available through Fireworks on **Microsoft Foundry**, offering a 1-million-token context window for long-horizon coding, document synthesis, and agentic tasks.
- **Multimodal generative video models via fal integration** *(In Preview)*\
  A curated portfolio of five generative video models—including Kling v3 Pro, LTX-2.5 Fast, LTX-2.5 Pro, MiniMax H3 Max, and MiniMax H3 Max Turbo—is now available in public preview as a first-party service in **Microsoft Foundry**. Developers can generate text-to-video and image-to-video outputs with synchronised audio and Microsoft Entra ID keyless authentication.
- **Real-Time Multichannel Speech-to-Text** *(Generally Available)*\
  **Azure Speech** now supports production real-time multichannel transcription with built-in per-channel language identification. Contact centre and conversational AI workloads can transcribe up to two independent audio channels within a single session at the same price as single-channel transcription.

## Compute & Containers

- **.NET 11 support for isolated worker model** *(Generally Available)*\
  **Azure Functions** now provides general availability support for targeting `.NET 11` (`net11.0`) in C# using the isolated worker model and the new `Azure.Functions.Sdk` project package. Note that support for the legacy in-process hosting model formally ended on 10th November 2026.
- **Cross-cluster networking via Azure Kubernetes Fleet Manager** *(Generally Available)*\
  **Azure Kubernetes Service (AKS)** cross-cluster networking managed through **Azure Kubernetes Fleet Manager** is now generally available. This enables managed east-west pod connectivity across multiple AKS clusters while multi-NIC pod support remains in public preview.
- **Support for .NET 8 and .NET 9 on Static Web Apps Ending** *(Retiring)*\
  Official platform support and security patches for `.NET 8` and `.NET 9` managed Functions APIs in **Azure Static Web Apps** ended on 10th November 2026. Workloads should be migrated to `.NET 10` (`dotnet-isolated:10.0`) on the isolated worker model to remain on a supported runtime.

## Databases & Storage

- **Modernize Arc-Enabled Windows Servers with Azure File Sync** *(In Preview)*\
  A new guided portal onboarding experience in **Azure Arc** streamlines agent installation, Storage Sync Service registration, and sync group configuration for Windows Server 2016 through 2025. Administrators can centrally configure cloud tiering and **Azure File Sync** endpoints directly from the Arc machine blade without manual RDP sessions.
- **Version store read metrics in Azure SQL Database** *(Generally Available)*\
  **Azure SQL Database** now exposes row version read counters across `STATISTICS IO`, `sys.dm_exec_requests`, `sys.dm_exec_sessions`, and query execution plans. Database administrators can directly quantify Read Committed Snapshot Isolation (RCSI) and Accelerated Database Recovery (ADR) version store overhead without requiring XPerf traces.

## Governance, Management & Developer Tools

- **Local CLI extension for Azure Logic Apps Standard** *(In Preview)*\
  The new `az logicapp` extension for **Azure Logic Apps** (Standard) brings 19 command groups and 64 commands to the local command-line interface. Developers and CI/CD pipelines can scaffold, validate, manage connectors, and run local workflows outside Visual Studio Code.
- **Scoped enforcement actions in Azure Policy for AKS** *(Generally Available)*\
  **Azure Policy** for Kubernetes now supports decoupling enforcement actions (`deny`, `audit`, or `warn`) from specific enforcement points (`audit.gatekeeper.sh`, `validation.gatekeeper.sh`, and native Kubernetes Validating Admission Policy `vap.k8s.io`). Platform teams can enforce API-server-level admission denials via VAP while using Gatekeeper webhooks as a fallback.

## Networking & Security

- **Azure Front Door edge actions** *(Generally Available)*\
  Edge actions in **Azure Front Door** are now generally available, allowing architects to execute custom routing, header manipulation, A/B testing, and dynamic origin selection logic directly at the global edge.
- **Azure Route Server dual-stack IPv4/IPv6 support** *(In Preview)*\
  **Azure Route Server** now supports dual-stack IPv4/IPv6 BGP peering in public preview, allowing route maps to be applied across ExpressRoute, VPN Gateway, and network virtual appliance (NVA) connections in dual-stack virtual networks.
- **Native gRPC support in Azure Front Door** *(In Preview)*\
  **Azure Front Door** now supports end-to-end gRPC traffic over HTTP/2 and HTTPS—including unary and streaming RPCs alongside dedicated gRPC health probes—in public preview.

That’s a wrap on this weeks Azure updates, if you found this helpful make sure to follow [blog.atozazure.com](http://blog.atozazure.com) for future updates, guides, and technical insights.