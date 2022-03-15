---
product: campaign
solution: Campaign 
title: Storage overview
description: Learn how to monitor in the Control Panel the different Campaign resources that are consuming database space on your instances.
feature: Control Panel
role: Architect
level: Experienced
exl-id: bb9e1ce3-2472-4bc1-a82a-a301c6bf830e
---
# Storage overview {#storage-overview}

>[!CONTEXTUALHELP]
>id="cp_dbdetails_storagedetails"
>title="About Storage overview"
>abstract="In this tab, you can get detailed information on the different Campaign resources that are consuming database space."

The **[!UICONTROL Storage overview]** area provides a graphical representation of the space occupied by:

* **[!UICONTROL System resources]**

    Note that, if system resources are consuming a large part of the database space, we recommend reaching out to Customer Care.

* **[!UICONTROL Out-of-the-box tables]** provided by default with your Campaign instances,
* **[!UICONTROL Temporary tables]** created by workflows and deliveries,
* **[!UICONTROL Non-out of the box tables]** generated after creating custom resources.

![](assets/database-storage-overview.png)

Click the **[!UICONTROL View details]** button to get more details on the different assets that are consuming database space.

You can use the drop-down list to refine your search and display tables from a specific asset type only (worklows, deliveries, recipients).  

![](assets/database-storage-details.png)

Note that this screen also allows you to clean and monitor workflow parameters that may require specific attention to avoid any issues on your instances. Learn more in [this page](workflow-monitoring.md).
