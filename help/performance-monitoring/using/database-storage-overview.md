---
product: campaign
solution: Campaign
title: Storage overview
description: Learn how to monitor in the Control Panel the different Campaign resources that are consuming database space on your instances.
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: bb9e1ce3-2472-4bc1-a82a-a301c6bf830e
TQID: 'https://experienceleague.adobe.com/3zcScy61C5LHsWM86WWWuy0uic-pdNQGKc0qY7ewwOQ'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
    internal-label: Administration
subfeature_v2:
  - id: e519a22f-a06a-42fc-9d09-d78a3ab2c434
    internal-label: Monitoring guidelines
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
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

Note that this screen also allows you to monitor workflow parameters that may require specific attention to avoid any issues on your instances. Learn more in [this page](workflow-monitoring.md).
