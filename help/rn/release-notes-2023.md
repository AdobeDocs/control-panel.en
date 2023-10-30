---
title: Release Notes 2023
description: This page lists all 2023 releases of Control Panel.
feature: Control Panel, Release Notes
role: Admin
level: Experienced
exl-id: 9a83e32a-4c11-4784-a6fe-341ce9ebc7a7
---
# Release Notes 2023 {#rn-2023}

## September 2023 {#september-2023}

<table>
<thead>
<tr>
<th><strong>DMARC & BIMI records management</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><p>You can now add DMARC & BIMI records directly from Control Panel:

<ul><li><strong>DMARC records</strong> provide a way to authenticate the sender's domain and prevent unauthorized use of the domain for malicious purposes. <a href="../subdomains-certificates/using/dmarc.md">Learn how to add DMARC records</a></li>
<li><strong>BIMI records</strong> allow you to display an approved logo next to your emails in mailbox providers' inboxes to enhance brand recognition and trust. <a href="../subdomains-certificates/using/bimi.md">Learn how to add BIMI records</a></li></ul>
</td>
</tr>
</tbody>
</table>

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
