---
title: "The A-Z of Azure: R is for Resource Groups"
seoTitle: "Azure Resource Groups Explained: A Guide to Logical Grouping"
seoDescription: "Organise Microsoft Azure workloads and manage lifecycles with Resource Groups. Learn cost optimisation best practices in this beginner cloud guide."
datePublished: 2026-05-10T13:06:08.257Z
cuid: cmozsdn9c00xa1qizcic63fck
slug: resource-groups
cover: https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/5deb4c94-32b1-47f1-aaee-c198faf9c62c.jpg
ogImage: https://cdn.hashnode.com/uploads/og-images/6862cf4acc277a35bb68ec0f/363307a1-e726-4e83-863d-7873f7a8d802.jpg
tags: microsoft, azure, fundamentals, microsoft-azure

---

### Introduction

Wondering how to keep your Azure environment organised and efficient? Following our guide on subscriptions, this entry breaks down Azure Resource Groups—the essential logical containers for your cloud resources. We explore the straightforward creation process, crucial nuances regarding metadata regions, and how grouping deployments by workload simplifies lifecycle management. Discover how mastering this foundational practice directly drives both Cost Optimisation and Operational Excellence within your cloud architecture.

### Getting Started

In the previous entry, we covered subscriptions, so naturally it makes sense that we now cover Resource Groups. In short, just like a subscription, you can think of a resource group as another sort of 'container', and these sit within or under your subscription (or subscriptions if you have multiple). However, unlike subscriptions, resource groups are primarily—as the name suggests—a method of grouping your deployed cloud resources, be that a virtual machine or a virtual network, into one logically assigned place.

How you logically group your cloud resources inside a Resource Group is up to you. Now, if you want to be a monster, you could 'technically' deploy everything into one single resource group and call it a day; however, it's no coincidence that Microsoft allows you to deploy up to 980 separate resource groups per Azure subscription. Instead, what is generally considered the best practice is that you group your resources by 'workload' or by 'application'—but what do I mean by that?

### Real-world example

Let's use a real-world example: You have a retail store on the high street that sells groceries. Would it make sense to have all your spare stock stored on the other side of town? No, probably not! Not only would it be very inefficient running back and forth, but it would also put the stock at risk of damage and potentially even loss. A similar concept applies here for Resource Groups.

Resource groups allow you to 'group' together the resources required for whatever it is you want to deploy. Sticking with the retail store, but this time it's an internet-hosted retail store: you would want to keep your product database with the other elements of the store—such as your Azure App Service or Static Web application that runs the actual visual element of your store—together. This ensures that for any maintenance work, you know exactly which resources are related to that specific web store.

### Creating a Resource Group

Creating a resource group is a very straightforward process. Simply open the Azure Portal and in the search bar type 'Resource Group'. It will appear in the drop-down list; then, simply click 'Create'. Once you're in the Basics menu, there are only a few options to choose from:

![](https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/3a4779cc-7de5-48a1-8479-93061497e679.png align="center")

Once you're in the Basics menu, there are only a few options to choose from:

*   **Subscription:** What subscription is the resource group being deployed to for billing purposes, you can read more about subscriptions [here](https://blog.atozazure.com/s-is-for-subscriptions)
    
*   **Resource group name:** What you want to call the resource group. Top tip: don't name it just 'Resource Group'—you'll regret it later.
    
*   **Region:** What region the resource group will be deployed too.
    

![](https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/94f9dd55-4838-44da-8093-9f6fe6d5a838.png align="center")

However, while these options seem very basic—and for the most part, they are—there are some nuances as a newcomer to the platform you should be aware of! The main one is region. Deploying a resource group **does not** dictate or control the region of the resources you can deploy into it. Resource Groups hold only the metadata; so, while your resource group could be deployed in UK South, you could still have a virtual machine deployed in Australia East within that same resource group.

> Best Practice: Always try to keep your resource group and its resources in the same region to ensure high availability of management operations and for compliance purposes\*\*.\*\*

With your subscription chosen and your region and resource group name selected, you then have the Tags menu that we'll cover in a future entry. For now, let's skip to **Review + Create** to then select 'Create' and complete our deployment. That's it—you have your very first Azure Resource Group!

![](https://cdn.hashnode.com/uploads/covers/6862cf4acc277a35bb68ec0f/6914c7c3-3de0-4f27-a8f4-3bb58243791e.png align="center")

### Lifecycle management

Remember earlier when I said you could technically add all your resources to a single resource group and call it a day? Well, another reason you might not want to do that is to ensure you are keeping good lifecycle management. What do I mean by that? Well, let's say your company is working on an experimental project and you create a bunch of different resources, from Virtual Machines and App Services to maybe even some sort of virtual network.

Now, when that experimental project concludes, those resources will not be needed anymore. Good practice is to then delete those resources to prevent any further spend. While you could dig through the list of resources if you had everything in one single resource group, there might be hidden resources or even some storage that gets missed. While a few missed resources that don't get deleted won't cost a lot in the best-case scenario (depending on what they are), over time those missed resources will build up and equal a much larger unnecessary spend.

Whereas, if we followed the recommended method and deployed resources into resource groups based on the workload or application, cleaning up is as simple as deleting a single resource group. Deleting the group removes all the corresponding resources for the project, ensuring that everything is cleaned up together.

### Closing thoughts

To wrap things up, think of Resource Groups as the glue that holds your Azure architecture together. While they might seem like a simple administrative boundary, they are actually your first line of defence in maintaining **Operational Excellence** and **Cost Optimisation**. By keeping your resources organised and logically grouped, you’re not just making your own life easier—you’re ensuring your cloud environment is scalable, secure, and doesn't break the bank with "forgotten" ghost resources. In the next post, we’ll be looking at **Tags**, which will give you even more granular control over your deployments. Until then, keep your subscriptions tidy and your regions consistent!