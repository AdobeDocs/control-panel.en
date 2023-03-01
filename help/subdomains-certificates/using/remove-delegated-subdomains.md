---
product: campaign
solution: Campaign 
title: Remove delegation of subdomains
description: Learn how to remove the delegation of subdomains to Adobe.
feature: Control Panel
role: Architect
level: Experienced
---
# Remove delegation of subdomains to Adobe {#remove-delegated--subdomains}

>[!CONTEXTUALHELP]
>id="cp_subdomain_undelegate"
>title="Remove subdomain delegation"
>abstract="This screen allows you to remove the delegation of a subdomain to Adobe. Keep in mind that this process cannot be undone and is irreversible until its execution is complete.<br><br>If you are trying to remove the delegation of a primary domain for the selected instance, you will be asked to choose the domain that will replace it."

Control Panel allows you to remove the delegation of a subdomain that has been delegated to Adobe, including CNAME setup.

## Important notes {#important}

Before proceeding, carefully consider the impacts occuring once the removal process is triggered:

* Once the process is triggered, subdomain delegation removal cannot be undone and is irreversible until the process execution is complete.
* No other subdomain delegation can be removed when a similar process on another subdomain is in progress.
* A delegation removed on a subdomain cannot be re-delegated until 3 days of its removal.

## Remove a subdomain delegation {#steps}

To remove the delegation of a subdomain to Adobe, follow these steps:

1. Click the ellipsis button next to the domain delegation you want to remove and select **[!UICONTROL Remove delegated subdomain]**.

    ![](assets/undelegate-subdomain.png)

1. Review the disclaimer and acknowledge the removal of the domain delegation to Adobe.

1. Review information regarding the instance to which the subdomain is associated, including related IP affinities and brand configurations.

    If you are removing the delegation of the primary domain for the selected instance, you need to choose the domain that will replace it using the **[!UICONTROL Replacement Domain]** list.
    
    Click **[!UICONTROL Next]** to proceed with the removal.

    ![](assets/undelegate-subdomain-details.png)

1. Review the summary that displays. To confirm the removal, type the URL of the domain for which you want to remove the delegation and click **[!UICONTROL Submit]**.

    ![](assets/undelegate-submit.png)

After delegation removal has been started, the pending job displays in the job logs until it is completed.

![](assets/undelegate-job.png)

## Error codes {#FAQ}

This section lists the error messages that you may encounter when trying to remove the delegation of a subdomain:

|Error code|Message|Description|
|  ---  |  ---  |  ---  |
|8002|Requested Delegated Domain removal cannot be addressed as there is an similar overlapping request in progress, please try after 3 days|A subdomain delegation removal job is already under process for the selected instance. Wait until 3 days to start a new removal job.|
|8003|Requested Delegated Domain removal is unsupported for this instance.|Delegation removal is not supported for the selected subdomain due to a technical issue, reach out to Customer Care.|
|8004|Requested Delegated Domain removal is not allowed as there is only one domain in this instance.|Only one subdomain has been delegated for the selected instance. Delegation removal is not allowed.|
|8005|Requested Delegated Domain removal is not supported for this configuration.|Delegation removal is not supported for the selected subdomain due to a technical issue, reach out to Customer Care.|
|8006|Requested Delegated Domain removal is not allowed due to unknown reasons. Please contact customer care.|Delegation removal is not supported for the selected instance due to unknown issues, reach out to Customer Care.|
