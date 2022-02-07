---
product: campaign
solution: Campaign 
title: Monitoring active queries
description: Learn how to monitor active queries on your Campaign instances in the Control Panel.
feature: Control Panel
role: Architect
level: Experienced
---
# Monitoring active queries {#long-running-queries}

The **[!UICONTROL Active queries]** area from the **[!UICONTROL Databases]** tab lists the five queries that have been running for the longest time on the selected intance.

![](assets/active-queries.png)

The **[!UICONTROL Duration]** columns specifies for how long a query has been running on the instance. Duration displays in this format: `hh:mm:ss.ms`.

>[!IMPORTANT]
>
>If one of the queries has been active for more than 24 hours, you will be notified by email if you subscribed to [email alerting](email-alerting.md).
>
>In that case, reach out to Customer Care so that they identify and resolve the issue. You will need to provide them with the **[!UICONTROL PID]** column value, which is a unique identifier for the query.