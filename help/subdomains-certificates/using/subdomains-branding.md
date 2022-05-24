---
product: campaign
solution: Campaign 
title: Subdomains branding
description: Learn more about subdomains branding
feature: Control Panel
role: Architect
level: Intermediate
exl-id: a489d051-fb95-45cf-bb6d-33aef10b7795
---
# Subdomains branding {#subdomains-branding}

>[!CONTEXTUALHELP]
>id="cp_certificate_management"
>title="About subdomains and SSL certificates"
>abstract="Monitor your subdomains and the associated SSL certificates."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/monitoring-ssl-certificates.html" text="Monitoring SSL certificates"

## Why setting up subdomains? {#why-setting-up-subdomains}

A subdomain is a division of your domain that can be used to isolate your brands, or various types of traffic (transactional messages, marketing information, etc.).

Let's take the example of the "mybrand.com" domain, that is used to send both transactional and marketing communications. In this situation, you can decide to set up two subdomains:

* "info.mybrand.com" subdomain for your transactional communications (purchases confirmation, password reset, etc.),
* "marketing.mybrand.com" subdomain for your prospecting emailings.

By doing so, you will help preserve the reputation of your domain and other subdomains. For example, if the "marketing.mybrand.com" subdomains ended up being added to the block list by Internet Service Providers due to bad deliverability, this would prevent the whole "mybrand.com" domain and the "info.mybrand.com" subdomain from being added to the block list.

## Subdomain configuration methods {#subdomain-delegation-methods}

Subdomain configuration allows you to configure a sub-section of your domain (technically a "DNS zone") for use with Adobe Campaign. Available setup methods are:

* **Full subdomain delegation to Adobe Campaign** (recommended): The subdomain is fully delegated to Adobe. Adobe is able to deliver the Campaign as a managed service by controlling and maintaining all aspects of DNS that are required for delivering, rendering and tracking of email campaigns.

* **Use of CNAMEs**: Create a subdomain and use CNAMEs to point to Adobe-specific records. Using this setup, both Adobe and the customer share responsibility for maintaining DNS.

The table below provides a summary of how these methods work, as well as the implied level of effort:

| Configuration method | How it works | Level of effort |
|---|---|---|
| **Full delegation** | Create the subdomain and namespace record. Adobe will then configure all DNS records required for Adobe Campaign.<br/><br/>In this setup, Adobe is fully responsible for managing the subdomain and all the DNS records. | Low |
| **CNAME, custom method** |  Create the subdomain and namespace record. Adobe will then provide the records to be placed in your DNS servers and will configure the corresponding values in Adobe Campaign DNS servers.<br/><br/>In this setup, both you and Adobe share responsibility for maintaining DNS. | High |

Additional information on domain configuration is available in [this documentation](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/product-specific-resources/campaign/ac-domain-name-setup.html).

If you have any question regarding subdomain configuration methods, reach out to Adobe Deliverability team, or eventually contact Customer Care to request Deliverability consulting.

## Subdomains' use cases (Campaign v7/v8){#subdomains-use-cases}

>[!CONTEXTUALHELP]
>id="cp_add_subdomain_usecase_selection"
>title="Select the use case for your subdomain"
>abstract="Breaking down your subdomains by use cases is a best practice for deliverability. By doing so, the reputation of each subdomain is isolated and protected."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/setting-up-new-subdomain.html" text="Setting up a new subdomain"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html" text="Subdomains branding"

When setting up subdomains for Campaign v7/v8 instances, you are required to select the use case for which the subdomain will be used (see [Setting up a new subdomain](../../subdomains-certificates/using/setting-up-new-subdomain.md)).

Possible use cases are:

* **Marketing communications**: communications that are intended for a commercial purpose. Example: sales email campaign.

* **Transactional & operational communications**: transactional communications contain information aimed at completing a process that the recipient has started with you. Example: purchase confirmation, password reset email. Organizational communications relate to the exchange of information, ideas, and views within and outside the organization, with no commercial purpose.

**Breaking down your subdomains according to use cases is a best practice for deliverability**. By doing so, the reputation of each subdomain is isolated and protected. For example, if your subdomain for marketing communications ends up being added to the block list by Internet Service Providers, your transactional communications subdomain will not be impacted, and will keep being able to send communications.

**You can configure a subdomains for both Marketing and Transactional use cases**:

* For Marketing use cases, subdomains will be configured on **MID** (Mid sourcing) instances.
* For Transactional use cases, subdomains will be configured on ALL **RT** (Message Center / Real-time messaging) instances to ensure connectivity. The subdomains will therefore operate with all your RT instances.

>[!NOTE]
>
>If you are using Campaign v7/v8, Control Panel allows you to see what RT/MID instances are connected to the Marketing instance that you are working with. For more on this, refer to the [Instance Details](../../instances-settings/using/instance-details.md) section.

**Related topics:**

* [Setting up a new subdomain](../../subdomains-certificates/using/setting-up-new-subdomain.md)
* [Monitoring your subdomains](../../subdomains-certificates/using/monitoring-subdomains.md)
