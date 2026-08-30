---
title: "T is for Tags"
seoTitle: "Azure Tagging Strategy Guide: Governanc & Best Practice"
seoDescription: "Implement an enterprise Azure tagging strategy. Align metadata with the WAF, enforce Azure Policy, and reduce cloud costs."
datePublished: 2026-08-15T08:34:02.262Z
cuid: cmsu4dcp000000aj9fcpm961r
slug: t-is-for-tags
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/47544996-da11-410c-931d-e936ab937c52.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/d6fbbc18-73fc-4f03-ace3-2a6abfdc56a2.png

---

### Introduction

In our previous entry covering Resource Groups, you might recall that we skipped right past the 'Tags' menu during our deployment. I promised we would cover them in a future post, noting that they give you even more granular control over your deployments. Well, the time has come to make good on that promise.If Subscriptions and Resource Groups are the physical containers defining the boundaries of your cloud environment, Tags are the labels on the outside of those boxes that tell you exactly what is inside, who owns it, and how important it is.

### What are Azure Tags?

At their core, Azure Tags are simple metadata elements consisting of a **Key** and a **Value** pair.

Think of it like filing a document. The 'Key' is the category (e.g., `Department`), and the 'Value' is the specific detail (e.g., `Finance`). You apply these key-value pairs directly to your Azure resources, resource groups, or even entire subscriptions.

While clicking around the Azure Portal and adding tags manually is fine for a single sandbox environment, in an enterprise scenario, this metadata becomes the lifeblood of your cloud management strategy. When adopting the Microsoft Cloud Adoption Framework (CAF), a robust tagging strategy is mandatory for proper governance and resource organisation.

### Aligning Tags with the Well-Architected Framework (WAF)

To truly understand the power of tags, we need to look beyond simply labelling things and see how they drive enterprise-grade automation and AI integration. Here is how a solid tagging strategy directly supports the five pillars of the Microsoft Well-Architected Framework:

*   **Cost Optimisation:** This is often the primary driver for tagging. By tagging resources with keys like `CostCentre`, `ProjectCode`, or `Environment`, you can filter your Azure billing reports to see exactly how much your testing environment is costing compared to production. It allows finance teams to automate cross-charging across the business without having to decipher cryptic resource names.
    
*   **Operational Excellence:** This is where tags shine for automation. When building CI/CD pipelines, your DevOps tools can query tags to perform automated tasks. For instance, an automated script can look for all virtual machines tagged `Environment: Dev` and shut them down at 7:00 PM every evening to save money, automatically starting them again at 8:00 AM.
    
*   **Security:** Tags are vital for data classification and governance. By applying a tag like `DataClassification: Confidential`, you can use Azure Policy to automatically enforce stricter security controls, ensuring that highly sensitive resources cannot be accidentally exposed to the public internet.
    
*   **Reliability:** In a disaster recovery scenario, you need to know what to restore first. Tagging resources with `Criticality: Tier1` or `Criticality: Tier3` allows your automated recovery runbooks to prioritise mission-critical workloads over lower-priority internal tools, ensuring your business gets back online efficiently.
    
*   **Performance Efficiency:** Tags help in grouping resources to monitor performance telemetry. By tagging a web app, its backend database, and its storage account with an identical `ApplicationName: CustomerPortal` tag, you can aggregate Azure Monitor metrics across all related components to identify performance bottlenecks holistically.
    

### Real-World Example

Let's stick with the retail store example we used when discussing Resource Groups.

Imagine your retail company has expanded massively. You now have hundreds of microservices, databases, and AI-driven inventory prediction tools scattered across your cloud environment.

If an engineer needs to update the stock-taking application, they don't want to accidentally apply an automated patch to the live checkout system. By enforcing a tagging policy, every resource tied to the stock system might carry the tags:

*   `Application: InventoryPredictor`
    
*   `Environment: Production`
    
*   `Owner:` [`retail-dev-team@company.co.uk`](mailto:retail-dev-team@company.co.uk)
    

Now, when your automated deployment pipelines run, they specifically target resources matching those exact metadata criteria, entirely mitigating the risk of human error.

### Creating/ Deploying Tags

### How to Enforce a Tagging Strategy

As your cloud footprint grows, relying on engineers to manually remember to add tags will inevitably lead to mistakes.

The enterprise standard is to enforce your tagging strategy using **Azure Policy**. You can configure a policy that dictates, for example, "No resource can be created in this subscription unless it has a 'CostCentre' tag." If an engineer attempts to deploy a resource via the portal, Bicep, or Terraform without that tag, the deployment will automatically fail, returning an error explaining the missing requirement.

Furthermore, you can set up policies that automatically *inherit* tags. If you tag a Resource Group with `Department: Marketing`, any new storage account or virtual machine deployed into that group can automatically inherit that tag, ensuring compliance with zero extra effort from your engineers.

### Closing Thoughts

While they might seem like a minor administrative detail during a deployment, Tags are the foundation of mature cloud governance. They transform a chaotic list of servers and databases into a highly structured, automated, and trackable enterprise environment.

Take the time to define your tagging strategy early. A well-planned taxonomy will save you endless headaches when you start scaling your automation, auditing your security, or trying to explain your monthly Azure bill to the finance department!