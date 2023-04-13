---
product: campaign
solution: Campaign
title: Throughputs and latency monitoring
description: Learn how to monitor your Campaign instances throughputs and latency in the Control Panel.
feature: Control Panel
role: Architect
level: Experienced
exl-id: eddef17f-0667-4b43-bc56-2b1aeeae61bb
---
# Throughputs and latency monitoring {#throughputs-latency-monitoring}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_throughputslatencies"
>title="About throughputs and latency monitoring "
>abstract="In this tab, you can monitor how delivery throughputs and latency are trending over a period of time on your instances. For information about deliveries contributing to the throughput, switch to tabular view."

Control Panel allows you to monitor delivery throughputs and latency for each of your instances.

>[!IMPORTANT]
>
>This feature is available to all Campaign Standard, v8 customers, and to Campaign v7 customers with build numbers 9032 and newer, including [standalone deployments](https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/deployment-types-/standalone-deployment.html) (without any mid instance).

Monitoring how delivery throughputs and latency are trending over a period of time is essential to understand the usage of your instances and ensure they are performing well.

This information is made available in Control Panel for each of your Campaign instances in the **[!UICONTROL Performance Monitoring]** card, **[!UICONTROL Throughputs & Latency]** tab (note that the Control Panel may take up to 1 hour to display the figures).

>[!NOTE]
>
>All figures presented in this area are approximate and for information purposes only.

![](assets/throughput-latencies-overview.png)

By default, data is displayed for the current day. You can change the displayed period of time using the **[!UICONTROL 6 months]**, **[!UICONTROL 30 days]** and **[!UICONTROL 7 days]** buttons. Data will be presented:
* Hourly for 1 day and 7 days view,
* 6 hourly for 30 days view,
* Daily for 6 months view.

You can also visualize information in a tabular format with sortable columns rather than a graph. To do this, click the **[!UICONTROL Visualization settings]** button then select **[!UICONTROL Table]**.

![](assets/throughput-latencies-table.png)

## Monitor throughput {#throughput}

The **[!UICONTROL Throughput]** area provides information regarding the number of messages sent per hour from the selected Campaign instance for all the communication channels that you are entitled to.

>[!NOTE]
>
>For Campaign v7/v8, throughput number shown is the throughput achieved from MID (mid sourcing) instances. For standalone marketing (MKT) deployments (without any MID instance), throughput from MKT instance is shown instead.

Aditionally, Control Panel allows you to identify the IDs of the top 5 deliveries that are contributing to the throughput for the selected period of time. This information is available in tabular view only:

![](assets/throughput-latencies-top5.png)

## Monitor Latency {#latency}

The **[!UICONTROL Latency]** area provides information regarding the latency encountered on the selected instance when sending real-time transactional communications.

>[!NOTE]
>
>Note that information related to **Profile Latency** is also available for [!DNL Campaign Standard] instances only.

Latencies are captured and visualized at 95 and 99 percentile, meaning that 95% and 99% of the requests should be faster than the given latency.

![](assets/throughput-latencies-latency.png)

By default, latency is shown for all channels. You can visualize latency for a specific channel using the drop-down list.

![](assets/throughput-latencies-filter.png)

>[!NOTE]
>
>Channel filtering is available for Campaign Classic v7/v8 instances only.
