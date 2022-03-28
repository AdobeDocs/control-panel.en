---
product: campaign
solution: Campaign 
title: Control Panel releases
description: This page lists all the new features and improvements for Control Panel
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
---
# Control Panel releases {#control-panel-releases}

This page lists all the new features and improvements for Control Panel.

>[!NOTE]
>
>Control Panel is accessible to Admin users only. Learn more about permissions in [this section](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html#discover-control-panel).
>
>For Campaign v7, your instance must be hosted on Amazon Web Services (AWS) and upgraded to the latest [Campaign stable build](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/rn-overview.html#rn-statuses) (or to build 9032 or higher). Learn how to check your version in [this section](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html#getting-your-campaign-version). To check if your instance is hosted on AWS, follow the steps detailed in [this page](faq.md#hosted-aws).

## March 2022 {#march-2022}

### New capabilities 

<table>
<thead>
<tr>
<th><strong>Clean paused and completed workflows</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel now allows you to identify paused and completed workflows and clean the temporary resources generated on your instances.</p><p>For more information, refer to the <a href="performance-monitoring/using/workflow-monitoring.md#clean">detailed documentation.</a></p>
</td>
</tr>
</tbody>
</table>


## February 2022 {#february-2022}

<table>
<thead>
<tr>
<th><strong>Workflow parameters monitoring</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now monitor workflow parameters that may require specific attention to avoid any issues on your instances. </p><p>For more information, refer to the <a href="performance-monitoring/using/workflow-monitoring.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## January 2022 {#january-2022}

<table>
<thead>
<tr>
<th><strong>Active queries monitoring</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel now allows you to monitor queries that have been running for the longest time on your instances.</p><p>For more information, refer to the <a href="performance-monitoring/using/database-active-queries.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Throughputs and latency monitoring</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now monitor how delivery throughputs and latency are trending over a period of time on your instances.</p><p>For more information, refer to the <a href="performance-monitoring/using/thoughputs-latencies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>SSL certificates operations on new subdomains</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>SSL certificates operations can now be performed on a newly set up subdomain, even if the deliverability audit is still in progress.</p><p>For more information, refer to the <a href="subdomains-certificates/using/renewing-subdomain-certificate.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## October 2021 {#october-2021}

<table>
<thead>
<tr>
<th><strong>IP range and public key validity period</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>It is now possible to set a duration for the availability of IP ranges and public keys. </p><p>For more information, refer to the <a href="sftp/using/ip-range-allow-listing.md#adding-ip-addresses-allow-list">IP range allow listing</a> and <a href="sftp/using/key-management.md#installing-ssh-key">Key management</a> sections.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>IP range and public key edition</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now edit the <a href="sftp/using/ip-range-allow-listing.md#editing-ip-ranges">IP ranges</a> and <a href="sftp/using/key-management.md#editing-public-keys">public keys</a> that you create. Note that this feature is not available for the items created before the current Control Panel release.
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Alerting on SFTP IP range and public key expiry</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The email alerting functionality now includes alerts on SFTP IP allow listing expiration and SFTP public key expiration.</p><p>For more information, refer to the <a href="performance-monitoring/using/email-alerting.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Full support with Campaign v8</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The <strong>Subdomain</strong> and <strong>Certificate</strong> management capabilities are now supported by Control Panel on Adobe Campaign v8.</a>.</p>
</td>
</tr>
</tbody>
</table>

## August 2021 {#august-2021}

<table>
<thead>
<tr>
<th><strong>Support with Campaign v8</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel is now available for Adobe Campaign v8, except the <strong>Subdomain</strong> and <strong>Certificate</strong> management capabilities, which are not yet supported.</p><p>For more information, refer to the <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/deploy/self-service.html" target="blank">Campaign v8 documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## October 2020 {#october-2020}

<table>
<thead>
<tr>
<th><strong>Subdomain configuration using CNAMEs</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel now allows you to configure a subdomain to work with Adobe using CNAMEs directly from the interface.</p><p>For more information, refer to the <a href="subdomains-certificates/using/setting-up-new-subdomain.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Database monitoring enhancements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Database monitoring has been enhanced with additional metrics that allow you to get detailed information on the resources that are consuming space on your database.</p><p>For more information, refer to the <a href="performance-monitoring/using/database-monitoring.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## June 2020 {#june-2020}

<table>
<thead>
<tr>
<th><strong>Subdomain deliverability audit</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>After delegating a new subdomain, Control Panel now allows you to track the audit performed by the Deliverability team.</p><p>For more information, refer to the <a href="subdomains-certificates/using/setting-up-new-subdomain.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>GPG keys management</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel now allows you to generate a pair of GPG keys, so you can easily decrypt the data coming to Campaign from the outside. In addition, we have added a capability so you can install a public GPG key to encrypt data leaving Campaign.</p><p>For more information, refer to the <a href="instances-settings/using/gpg-keys-management.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Active profiles monitoring</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel now allows you to monitor the number of active profiles that are used by your instances and counted for billing purposes.</p><p>For more information, refer to the <a href="performance-monitoring/using/active-profiles-monitoring.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

>[!IMPORTANT]
>
>Active profiles monitoring from the Control Panel is available in beta, and subject to frequent updates and modifications without notice.

## May 2020 {#may-2020}

<table>
<thead>
<tr>
<th><strong>Certificate management for CNAME subdomains</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel now allows you to renew the SSL certificates of your subdomains that have been configured with the CNAME method.</p><p>For more information, refer to the <a href="subdomains-certificates/using/renewing-subdomain-certificate.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## April 2020 {#april-2020}

<table>
<thead>
<tr>
<th><strong>Google TXT record management</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Add Google TXT site verification record to all your subdomains used to send emails to Gmail addresses through the Campaign Control Panel.</p><p>For more information, refer to the <a href="subdomains-certificates/using/managing-txt-records.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Database space monitoring</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign Control Panel is equipped with database monitoring capabilities, allowing you to view your database space utilization on-demand and over time.</p><p>For more information, refer to the <a href="performance-monitoring/using/database-monitoring.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Email alerting</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign Control Panel is equipped with real-time email alerting capabilities, allowing you to login to the Control Panel and sign up to receive alerts when your system is at risk of performance deterioration, or an action is required to ensure high performance for the future.</p><p>For more information, refer to the <a href="performance-monitoring/using/email-alerting.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## January 2020 {#january-2020}

We’ve added new capabilities for Admin users to configure subdomains and renew SSL certificates from Control Panel.

For more information, refer to these pages:
* [Setting up a new subdomain](subdomains-certificates/using/setting-up-new-subdomain.md)
* [Renewing a subdomain's SSL certificate](subdomains-certificates/using/renewing-subdomain-certificate.md)

>[!IMPORTANT]
>
>These features will be available in beta, and subject to frequent updates and modifications without notice.

## September 2019 {#september-2019}

We’ve added new capabilities for Admin users to add IP addresses to the allow list in order to connect to Campaign v7/v8 instances.
Additionally, Admin users can now view the list of Campaign v7/v8 instances and eligibility for build upgrades.

For more information, refer to the [dedicated documentation](instances-settings/using/ip-allow-listing-instance-access.md).

## August 2019 {#august-2019}

We’ve added new capabilities for Admin users to receive notifications before SSL certificates for their domains expire. For more information, refer to the [detailed documentation](subdomains-certificates/using/monitoring-ssl-certificates.md).

Additionally, Admin users can now delete SSH keys that were added to access SFTP servers.

## July 2019 {#july-2019}

We've added new features to empower Admin users to take greater control of Campaign v7/v8 instance settings. New Control Panel capabilities include the ability to add URLs that Adobe Campaign connect to for data/file transfers.

For more information, refer to the [detailed documentation](instances-settings/using/url-permissions.md).
