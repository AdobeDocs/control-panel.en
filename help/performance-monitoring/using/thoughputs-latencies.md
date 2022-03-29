---
product: campaign
solution: Campaign
title: Throughtputs and latency monitoring
description: Learn how to monitor your Campaign instances throughputs and latency in the Control Panel.
feature: Control Panel
role: Architect
level: Experienced
exl-id: eddef17f-0667-4b43-bc56-2b1aeeae61bb
---
# Throughtputs and latency monitoring {#throughputs-latency-monitoring}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_throughputslatencies"
>title="About throughputs and latency monitoring "
>abstract="In this tab, you can monitor how delivery throughputs and latency are trending over a period of time on your instances."

Control Panel allows you to monitor delivery throughputs and latency for each of your instances.

>[!IMPORTANT]
>
>This feature is available to all Campaign Standard and v8 customers, and to Campaign V7 customers with build number 9032 or 9330 that have [standalone](https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/deployment-types-/standalone-deployment.html) deployments (without any mid instance).

Monitoring how delivery throughputs and latency are trending over a period of time is essential to understand the usage of your instances and ensure they are performing well.

This information is made available in Control Panel for each of your Campaign instances in the **[!UICONTROL Performance Monitoring]** card, **[!UICONTROL Throughputs & Latency]** tab (note that the Control Panel may take up to 1 hour to display the figures).

* The **[!UICONTROL Throughput]** area provides information regarding the number of messages sent per hour from the selected Campaign instance for all the communication channels that you are entitled to.

    >[!NOTE]
    >
    >For Campaign v7/v8, throughput number shown is the throughput achieved from MID (mid sourcing) instances. For standalone marketing (MKT) deployments (without any MID instance), throughput from MKT instance is shown instead.

* The **[!UICONTROL Latency]** area provides information regarding the latency encountered on the selected instance when sending real-time transactional communications. Latencies are captured and visualized at 95 and 99 percentile, meaning that 95% and 99% of the requests should be faster than the given latency.

![](assets/throughput-latencies-overview.png)

>[!NOTE]
>
>All figures presented in this area are approximate and for information purposes only.

By default, data is displayed for the current day. You can change the displayed period of time using the **[!UICONTROL 6 months]**, **[!UICONTROL 30 days]** and **[!UICONTROL 7 days]** buttons.

You can also visualize information in a tabular format with sortable columns rather than a graph. To do this, click the **[!UICONTROL Visualization settings]** button then select **[!UICONTROL Table]**.

![](assets/throughput-latencies-table.png)
