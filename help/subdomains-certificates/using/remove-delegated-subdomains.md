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
>title="Subdomain delegation removal"
>abstract="This screen allows you to remove the delegation of a subdomain to Adobe. Keep in mind that subdomain delegation removal cannot be undone and will be irreversible once submitted.<br><br>If you are trying to remove the delegation of a primary domain for the selected instance, you will be asked to choose the domain that will replace it."

Control Panel allows you to remove the delegation of a subdomain that has been delegated to Adobe, including CNAME setup. Before proceeding, carefully consider the impacts occuring once the removal process is triggered:

* Subdomain delegation removal cannot be undone and will be irreversible once started,
* No other subdomain delegation can be removed when a similar process on another subdomain is in progress,
* A delegation removed on a subdomain cannot be re-delegated until about ~2 hours of its removal..

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
