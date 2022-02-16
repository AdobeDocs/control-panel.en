---
product: campaign
solution: Campaign
title: About database monitoring
description: Learn how to monitor your Campaign database in the Control Panel
feature: Control Panel
role: Architect
level: Experienced
exl-id: 2bd7d2dd-97be-49bb-9f8e-7161d0742bc1
---
# About database monitoring {#database-monitoring}

## About instances databases {#about-instances-databases}

According to your contract, each of your Campaign instances is provisioned with a specific amount of database space.

Databases include all **assets**, **workflows** and **data** that is stored in Adobe Campaign.

Over time, databases can reach their maximum capacity, especially if the stored resources are never deleted from the instance, or if there are many workflows in a paused state.

Overflowing an instance database can lead to several issues (inability to login, to send emails etc.). Monitoring your instances' databases is therefore essential to ensure optimal performance.

## Monitoring database usage{#monitoring-database-usage}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_database"
>title="About database monitoring"
>abstract="In this tab, you can get real-time information on the latest and historical database usage and evolution for each of your Campaign instances."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html" text="About performance monitoring"

Control Panel allows you to monitor the database usage for each of your Campaign instances. To do this, open the **[!UICONTROL Performance Monitoring]** card, then select the **[!UICONTROL Databases]** tab.

Select the desired instance from the **[!UICONTROL Instance List]** to display information about the instance's database capacity and used space.

Additionally, you can receive notifications when one of your databases is reaching its capacity. To do this, subscribe to [email alerts](../../performance-monitoring/using/email-alerting.md).

>[!NOTE]
>
>If the amount of available database space as shown in the Control Panel does not reflect the amount specified in your contract, reach out to Customer Care.

![](assets/databases_dashboard.png)

Data from this dashboard is updated based on the **[!UICONTROL Database cleanup technical workflow]** that runs on your Campaign instance (see [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html#list-of-technical-workflows) and [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/data-processing/database-cleanup-workflow.html) documentation). You can check the last time the workflow ran below the **[!UICONTROL Used Space]** and **[!UICONTROL Provided Space]** metrics. Note that, if the workflow has not been running since more than 3 days, we recommend reaching out to Adobe Customer care so that they investigate why the workflow is not running.

Additional metrics are available in this dashboard to help you analyse the usage of the instance's database. They are detailed in these sections:

* [Database utilization](../../performance-monitoring/using/database-utilization.md)
* [Storage overview](../../performance-monitoring/using/database-storage-overview.md)
* [Top 10 temporary resources](../../performance-monitoring/using/database-top-ten-resources.md)
* [Active queries](../../performance-monitoring/using/database-active-queries.md)

![](assets/do-not-localize/how-to-video.png) Discover this feature in video using [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/performance-monitoring/monitoring-databases.html#performance-monitoring) or [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/performance-monitoring/monitoring-databases.html#performance-monitoring)
