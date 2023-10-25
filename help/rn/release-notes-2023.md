---
title: Release Notes 2023
description: This page lists all 2023 releases of Control Panel.
exl-id: 9a83e32a-4c11-4784-a6fe-341ce9ebc7a7
---
# Release Notes 2023 {#rn-2023}

## October 2023 {#october-2023}

**User interface**

* Control Panel is now available in additional languages. [Learn more]()

**Active profiles monitoring**

* You can now monitor the number of active profiles you are entitled to for your organization, and the total count of profiles used in your organization within all instances, if you are using multiple instances. [Learn more](../performance-monitoring/using/active-profiles-monitoring.md)

**DMARC records**

* Multiple email addresses can now receive aggregate report and failure report emails. [Learn more](../subdomains-certificates/using/dmarc.md)
* Changes have been made if both DMARC and BIMI records exist for a subdomain:

    * DMARC records cannot deleted. If you want to delete one, you need to delete the BIMI record first.
    * DMARC records can be edited, but the policy downgrade to "None" is not allowed and its percentage value must be 100.

## June 2023 {#june-2023}

* You can now delegate the SSL certificates of already delegated subdomains to Adobe directly from the subdomains list. [Learn more](../subdomains-certificates/using/delegate-ssl.md)

* Alert Emails sender has been changed to `"alert@notifications.campaign.adobe.com"`.

## May 2023 improvements {#may-2023}

**Subdomains' SSL certificates delegation to Adobe**

You can now have your subdomains' SSL certificates managed by Adobe. If you are using CNAMEs to set up your subdomain, certificates records will be automatically generated and provided in order to generate a certificate into your domain hosting solution.

Note that this capability is only available when setting up a new subdomain. You cannot delegate certificates for existing delegated subdomains. [Learn more](../subdomains-certificates/using/setting-up-new-subdomain.md)

>[!NOTE]
>
>Adobe managed SSL is a cost-free feature that is available to users at no charge.

## March 2023 {#march-2023}

**Subdomain delegation removal for CNAMEs**

You can now remove the delegation of subdomains that have been configured using CNAMEs. [Learn more](../subdomains-certificates/using/remove-delegated-subdomains.md)

## February 2023 {#february-2023}

**Delegation removal for subdomains delegated to Adobe**

You can now remove the delegation of a subdomain that is fully delegated to Adobe. [Learn more](../subdomains-certificates/using/remove-delegated-subdomains.md)

>[!NOTE]
>
>Delegation removal is currently not available for subdomains that have been setup using CNAMEs.

**Service calendar**

Service calendar now provides a calendar view to keep track of important events occuring on your instances. In addition, information has been added on the notifications sent to users that subscribed to Control Panel alerts. [Learn more](../service-events/service-events.md)

![](assets/do-not-localize/gif-calendar.gif)

## January 2023 {#january-2023}

**New hybrid hosting model capability**

Customers with hybrid hosting model can now add IP addresses to the allow list for access to MID instances. [Learn more](../instances-settings/using/ip-allow-listing-instance-access.md)

**Certificate Signing Request (CSR) Enhancement**

The City/Locality field is now optional during Certificate Signing Request Generation.
