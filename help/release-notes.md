---
product: campaign
solution: Campaign 
title: Control Panel releases
description: Latest Control Panel release notes.
feature: Control Panel
role: Architect
level: Beginner
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
---
# Control Panel releases {#control-panel-releases}

Here you will find information about the latest Control Panel releases.

>[!NOTE]
>
>Control Panel is accessible to all Admin users. The steps to grant Admin access to a user are detailed in [this section](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=en#discover-control-panel).
>
>For Campaign Classic v7, note that your instance must be hosted on AWS and upgraded with the latest [Gold Standard](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/gs-release/gs-overview.html) build or the [latest GA build (21.1)](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/latest-release.html#release-notes). Learn how to check your version in [this section](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html#getting-your-campaign-version). To check if your instance is hosted on AWS, follow the steps detailed in [this page](faq.md).

## October 2021 {#october-2021}

You can now edit the [IP ranges](../../sftp/using/ip-range-allow-listing.md#editing-ip-ranges) and [public keys](../../sftp/using/key-management.md#editing-public-keys) that you create. Note that this feature is not available for the items created before the current Control Panel release.

It is now possible to set a duration for the availability of IP ranges and public keys. Read more in the [IP range allow listing](../../sftp/using/ip-range-allow-listing.md#adding-ip-addresses-allow-list) and [Key management](../../sftp/using/key-management.md#installing-ssh-key) sections

The email alerting functionality now includes alerts on SFTP IP allow listing expiration and SFTP public key expiration. [Read more](performance-monitoring/using/email-alerting.md)

The **Subdomain** and **Certificate** management capabilities are now supported by Adobe Campaign v8.

## August 2021 {#august-2021}

Control Panel is now available for Adobe Campaign v8, except the **Subdomain** and **Certificate** management capabilities, which are not yet supported. Learn more in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/deploy/self-service.html?lang=en){target="_blank"}

## October 2020 {#october-2020}

**Subdomain configuration using CNAMEs**

Control Panel now allows you to configure a subdomain to work with Adobe using CNAMEs directly from the interface. [Read more](subdomains-certificates/using/setting-up-new-subdomain.md)

**Database monitoring enhancements**

Database monitoring has been enhanced with additional metrics that allow you to get detailed information on the resources that are consuming space on your database. [Read more](performance-monitoring/using/database-monitoring.md)

## June 2020 {#june-2020}

**Subdomain deliverability audit**

After delegating a new subdomain, Control Panel now allows you to track the audit performed by the Deliverability team. [Read more](subdomains-certificates/using/setting-up-new-subdomain.md)

**GPG keys management** 

Control Panel now allows you to generate a pair of GPG keys, so you can easily decrypt the data coming to Campaign from the outside. In addition, we have added a capability so you can install a public GPG key to encrypt data leaving Campaign. [Read more](instances-settings/using/gpg-keys-management.md)

**Active profiles monitoring**

Control Panel now allows you to monitor the number of active profiles that are used by your instances and counted for billing purposes. [Read more](performance-monitoring/using/active-profiles-monitoring.md)

>[!IMPORTANT]
>
>Active profiles monitoring from the Control Panel is available in beta, and subject to frequent updates and modifications without notice.

## May 2020 {#may-2020}

**Certificate management for CNAME subdomains**

Control Panel now allows you to renew the SSL certificates of your subdomains that have been configured with the CNAME method. [Read more](subdomains-certificates/using/renewing-subdomain-certificate.md)

## April 2020 {#april-2020}

**Google TXT record management**

Add Google TXT site verification record to all your subdomains used to send emails to Gmail addresses through the Campaign Control Panel. [Read more](subdomains-certificates/using/managing-txt-records.md)

**Database space monitoring**

Campaign Control Panel is equipped with database monitoring capabilities, allowing you to view your database space utilization on-demand and over time. [Read more](performance-monitoring/using/database-monitoring.md)

**Email alerting**

Campaign Control Panel is equipped with real-time email alerting capabilities, allowing you to login to the Control Panel and sign up to receive alerts when your system is at risk of performance deterioration, or an action is required to ensure high performance for the future. [Read more](performance-monitoring/using/email-alerting.md)

## January 2020 {#january-2020}

*January 22, 2020*

We’ve added new capabilities for Admin users to configure subdomains and renew SSL certificates from Control Panel.

For more information, refer to these pages:
* [Setting up a new subdomain](subdomains-certificates/using/setting-up-new-subdomain.md)
* [Renewing a subdomain's SSL certificate](subdomains-certificates/using/renewing-subdomain-certificate.md)

>[!IMPORTANT]
>
>These features will be available in beta, and subject to frequent updates and modifications without notice.

## September 2019 {#september-2019}

*September 16, 2019*

We’ve added new capabilities for Admin users to add IP addresses to the allow list in order to connect to Campaign Classic instances.
Additionally, Admin users can now view the list of Campaign Classic instances and eligibility for build upgrades.

For more information, refer to the [dedicated documentation](instances-settings/using/ip-allow-listing-instance-access.md).

## August 2019 {#august-2019}

We’ve added new capabilities for Admin users to receive notifications before SSL certificates for their domains expire. For more information, refer to the [detailed documentation](subdomains-certificates/using/monitoring-ssl-certificates.md).

Additionally, Admin users can now delete SSH keys that were added to access SFTP servers.

## July 2019 {#july-2019}

We've added new features to empower Admin users to take greater control of Campaign Classic instance settings. New Control Panel capabilities include the ability to add URLs that Adobe Campaign connect to for data/file transfers.

For more information, refer to the [detailed documentation](instances-settings/using/url-permissions.md).
