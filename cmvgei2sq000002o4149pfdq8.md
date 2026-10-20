---
title: "The A-Z of Azure: M is for Management Groups"
seoTitle: "A Beginner's Guide to Management Groups in Azure "
seoDescription: "Learn what Azure Management Groups are, how they simplify RBAC, Policy, and Cost Management across subscriptions, and how to configure them."
datePublished: 2026-10-20T08:07:59.419Z
cuid: cmvgei2sq000002o4149pfdq8
slug: atozazure-management-groups
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/3866296e-2daa-43c4-a5dd-20c5ba8d2d18.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/3665ba9a-2869-4418-81c8-77d0cd0e91f3.jpg
tags: microsoft, azure, security, cloud-computing, devops, atozazure

---

## Introduction

Having previously looked at subscriptions in the series, I wanted to finish off the high-level governance piece (at least for a while) with 'Management Groups' as they go hand-in-hand with subscriptions, we'll cover what they are, what they do, and how you might configure them.

## What are Management Groups?

If you read the previous entry on [Subscriptions](https://blog.atozazure.com/atozazure-subscriptions) you might recall that I referred to them a kind of container, well that is also true of Management Groups. However unlike a subscription, Management groups dont hold resources they hold... \*Drumroll, Subscriptions! and because they hold subscriptions, that means that they sit one level higher in the topology structure.

By default, all Azure tenants contain what is known as a Tenant Root Group, think of it as your master management group if you will. Let's say for example you was to deploy another management group (or two), the new management group(s) would be nested underneath your 'Tenant Root Group' within the hierarchy as per the example diagram below.

![](https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/08002195-7a6e-42c6-aaa5-17f272327790.png align="center")

## What Are Management Groups For?

Okay, but why would I actually use management groups? Well, there are a number of reasons, including—but not limited to—some of the examples below. The magic word here is **inheritance**: anything you apply to a management group automatically cascades down to all the nested management groups, subscriptions, resource groups, and resources beneath it.

*   **Cost Management:** While billing technically happens at the subscription level, management groups allow you to aggregate costs and view consolidated spend across multiple subscriptions at once. If you have five different subscriptions for your 'Finance' department, putting them under a single 'Finance' management group lets you create unified budgets, track overall departmental spend, and run a single cost analysis report rather than stitching five separate spreadsheets together.
    
*   **RBAC (Role-Based Access Control):** Assigning permissions subscription-by-subscription gets tedious very quickly. With management groups, if your cloud platform team needs `Reader` or `Contributor` access across your entire estate, or your security team needs `Security Admin` across all production workloads, you simply assign the role once at the relevant management group level. Every current (and future!) subscription placed inside that group inherits those permissions automatically.
    
*   **Azure Policy:** This is arguably where management groups shine the brightest. Instead of applying governance guardrails piecemeal, you can enforce compliance at scale. For example, you might assign a policy at the **Tenant Root Group** restricting resource deployments exclusively to UK regions (`UK South` and `UK West`). Then, on a child **Production** management group, you could layer on stricter policies requiring specific cost-centre tags or enforcing geo-redundant backup SKUs, whilst leaving your **Sandbox** management group a bit more relaxed for testing.
    

## How Do You Configure Them?

Before you jump into the Azure Portal and start clicking around, it pays to do a little bit of whiteboard planning. Microsoft allows up to **10,000 management groups** in a single directory and a hierarchy up to **6 levels deep** (excluding the Tenant Root Group and the subscriptions themselves)—but just because you *can* go six levels deep doesn't mean you *should*!

If you don't have a physical whiteboard handy, I've built a free web-based [Management Group Planner Tool](https://app.atozazure.com/management-groups) that you can use to visually map out and test your hierarchy before deploying anything in Azure.

When planning your hierarchy, keep these two golden rules in mind:

*   **Organisational Alignment:** Structure your hierarchy to match how your business actually operates and governs its workloads. This could be broken down by **environment type** (e.g., *Production* vs. *Non-Production*—just like in the diagram above), **business unit** (e.g., *HR* vs. *Finance*), or **geography** (e.g., *UK* vs. *US*).
    
*   **Keep it Simple:** Avoid the trap of overcomplicating your tree or simply mirroring your company's HR org chart. A great starting point—aligned with Microsoft's Cloud Adoption Framework (CAF)—is a relatively flat structure dividing workloads into **Platform** (for shared services like networking and identity), **Landing Zones** (for your actual workloads, split by Prod/Dev), and **Sandbox** (for safe experimentation). Only add another layer of depth when you have a distinct Azure Policy or RBAC requirement that demands it.
    

### Creating a Management Group in the Portal

Once you know what your structure looks like, spinning one up is straightforward:

1.  Head to the **Azure Portal** and search for **Management groups** in the top search bar. *(Note: If it's your first time using them in a tenant, Azure will briefly initialise the Tenant Root Group for you).*
    
2.  Click **\+ Create** at the top left.
    
3.  Enter a **Management group ID** (this is the unique backend identifier and **cannot** be changed later, so choose wisely!) and a **Management group display name** (the friendly name you'll see in the portal, which you can rename anytime).
    
4.  Hit **Save**. By default, it will sit directly underneath your Tenant Root Group, or you can move it under an existing group by selecting the **...** menu next to it.
    
5.  Finally, to move a subscription inside your shiny new management group, click into the group, select **Subscriptions** from the left-hand menu, click **\+ Add**, and pick the subscription you want to govern from the drop-down list.
    

## Wrapping Up

And that's a wrap on Management Groups! Combined with Subscriptions and Resource Groups, you now have the complete blueprint for organising your Azure hierarchy from top to bottom. Getting this foundational structure right early on saves massive headaches down the line as your cloud footprint scales.