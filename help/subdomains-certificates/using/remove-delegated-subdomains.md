---
product: campaign
solution: Campaign 
title: Remove delegated subdomains
description: Learn how to remove subdomains that have been delegated.
feature: Control Panel
role: Architect
level: Experienced
---
# Remove delegated subdomains {#remove-delegated--subdomains}

>[!CONTEXTUALHELP]
>id="cp_subdomain_undelegate"
>title="Remove delegated subdomains "
>abstract="TBD"

## Must-read {#must-read}

Before starting, carefully consider the impacts below once the removal process is triggered for a subdomain:

Before removing a delegated subdomain, it is important to understand the following impacts once the removal process is triggered for a subdomain:

* Subdomain removal cannot be undone and will be irreversible once started,
* No other delegated subdomains can be removed until the removal process is complete,
* A removed subdomain cannot be re-delegated for the next 2 hours.

## Remove a delegate subdomain {#remove}

To remove a delegated subdomain, follow the steps below.

1. Click the ellipse button and select **[!UICONTROL Remove delegated subdomain]**.

    ![](assets/undelegate-subdomain.png)

1. Read the displayed disclaimer aknowledge the domain removal process.

1. Review the instance that is currently using the subdomain display along with related IP affinities and brand configurations.

    Select the subdomain to use in remplacement for the removed subdomain and select **[!UICONTROL Next]**.

    ![](assets/undelegate-subdomain-details.png)

1. A summary of the removal displays. Review it and type the url of the domain to remove to confirm.

    ![](assets/undelegate-submit.png)

1. Click **[!UICONTROL Submit]** to trigger the removal process.


