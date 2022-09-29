---
title: Release Notes 2022
description: This page lists all 2022 releases of Control Panel.
exl-id: 9fb18bb6-c4e4-48aa-849c-d9129add5266
---
# Release Notes 2022 {#rn-2022}

## August 2022 {#august-2022}

* Customers with hybrid hosting model can now verify their subdomains. [Learn more](../subdomains-certificates/using/monitoring-subdomains.md)
* Organization Unit (OU) field is now optional in Certificate Generation Request (CSR). [Learn more](../subdomains-certificates/using/renewing-subdomain-certificate.md)

## July 2022 {#july-2022}

<table>
<thead>
<tr>
<th><strong>Subdomains' cerfificates installation for hybrid hosting model</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><p>Customers with hybrid hosting model can now renew their subdomains' SSL certificates from the Control Panel.</p><p>For more information, refer to the <a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">detailed documentation.</a></p>
</td>
</tr>
</tbody>
</table>

## June 2022 {#june-2022}

### What's new?

<table>
<thead>
<tr>
<th><strong>Top 10 files consuming space on SFTP servers</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now identify the top 10 files that are consuming the most space on an SFTP server. <a href="../sftp/using/sftp-storage-management.md">Learn more</a></p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Service Calendar reminders</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Service Calendar now allows you to set reminders in order to be notified by email before an event is going to occur on your instances. <a href="../service-events/service-events.md">Learn more</a></p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Subdomains' CSR generation enhancements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Several enhancements have been made to the CSR generation process. <a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">Learn more</a></p><ul><li>When generating a CSR, you can now select one of the included subdomains as the Common Name.</li><li>You can now copy the CSR summary before generating the CSR.</li><li>Once a CSR has been generated, you can download it again from the job logs. This capability does not apply to certificates generated before this release.</li></ul><p>

</td>
</tr>
</tbody>
</table>

### Improvements

**Instances settings**

* The maximum number of GPG keys in Control Panel has been increased to 60 keys. [Learn more](../instances-settings/using/gpg-keys-management.md)

## May 2022 {#may-2022}

<table>
<thead>
<tr>
<th><strong>Control Panel availability to hybrid hosting model</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Control Panel is now available to customers with hybrid hosting model. These customers can leverage the features of Control Panel by providing their MID/RT instance URL configured in their marketing instance in Control Panel.</p><p>For more information, refer to the <a href="../instances-settings/using/external-accounts.md">detailed documentation.</a></p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Throughputs and latencies monitoring updates</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Throughputs and latencies monitoring capabilities have been enhanced:<ul><li>You can now identify the IDs of the top 5 deliveries that are contributing to the throughput of your instance.</li><li>Campaign Classic v7/v8 customers can now visualize latency for a specific channel.</p></li><p>For more information, refer to the <a href="../performance-monitoring/using/thoughputs-latencies.md">detailed documentation.</a></p>
</td>
</tr>
</tbody>
</table>


## April 2022 {#april-2022}

<table>
<thead>
<tr>
<th><strong>Monitor key contacts and events on your instances</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now monitor past and upcoming releases and service reviews occurring on your instances, as well as access a list of key contacts at Adobe for any request or issue.</p><p>For more information, refer to the <a href="../service-events/service-events.md">detailed documentation.</a></p>
</td>
</tr>
</tbody>
</table>

## March 2022 {#march-2022}

<table>
<thead>
<tr>
<th><strong>Throughputs and latency monitoring availability</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Throughputs and latency monitoring is now available to all Campaign Standard and v8 customers, and to Campaign V7 customers with build numbers 9032,9330, 9346 or 9349 that have standalone deployments (without any mid instance).</p><p>For more information, refer to the <a href="../performance-monitoring/using/thoughputs-latencies.md">detailed documentation.</a></p>
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
<p>You can now monitor workflow parameters that may require specific attention to avoid any issues on your instances. </p><p>For more information, refer to the <a href="../performance-monitoring/using/workflow-monitoring.md">detailed documentation</a>.</p>
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
<p>Control Panel now allows you to monitor queries that have been running for the longest time on your instances.</p><p>For more information, refer to the <a href="../performance-monitoring/using/database-active-queries.md">detailed documentation</a>.</p>
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
<p>You can now monitor how delivery throughputs and latency are trending over a period of time on your instances.</p><p>For more information, refer to the <a href="../performance-monitoring/using/thoughputs-latencies.md">detailed documentation</a>.</p>
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
<p>SSL certificates operations can now be performed on a newly set up subdomain, even if the deliverability audit is still in progress.</p><p>For more information, refer to the <a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
