---
product: campaign
solution: Campaign 
title: Active profiles monitoring
description: Learn how to get real-time information on the latest and historical Active Profiles usage and evolution for each of your Campaign instances.
feature: Control Panel
role: Architect
level: Experienced
exl-id: a157cc27-577f-490f-8c4f-0f203219cfb5
---
# Active profiles monitoring {#active-profiles-monitoring}

## About active profiles {#about-active-profiles}

>[!IMPORTANT]
>
>Active profiles monitoring from the Control Panel is available in beta, and subject to frequent updates and modifications without notice. It is available from Campaign Standard 10368 build.

According to your contract, each of your Campaign instances is provisioned with a specific amount of active profiles that are counted for billing purposes. Please refer to your latest contract for reference on number of purchased active profiles.

“Profile” means a record of information (e.g.: a record in the nmsRecipient table or an external table containing a cookie ID, Customer ID, mobile identifier or other information relevant to a particular channel) representing an end-customer, prospect, or lead.

Profiles are considered active if they have been targeted or communicated with in the past 12 months via any channel.

>[!NOTE]
>
>Facebook and Twitter channels are not taken into account.

For more on active profiles, refer to [Campaign Standard](https://https://experienceleague.adobe.com/docs/campaign-standard/using/profiles-and-audiences/managing-profiles/active-profiles.html) and [Campaign Classic v7](https://https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/profile-management/about-profiles.html#active-profiles) documentations.

## Monitoring active profiles {#monitoring-active-profiles}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_active_profile"
>title="About active profiles monitoring"
>abstract="In this tab, you can get real-time information on the latest and historical active profiles usage and evolution for each of your Campaign instances."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=en" text="About performance monitoring"

Control Panel allows you to monitor the active profiles usage for each of your Campaign instances.

To do this, follow these steps:

1. Open the **[!UICONTROL Performance Monitoring]** card, then select the **[!UICONTROL Active Profiles]** tab.

1. Select the desired instance from the **[!UICONTROL Instance List]**.

1. The number of active profiles used by the instance displays, as well as the last time the billing workflow was run on your instance.

![](assets/active-profiles-graph.png)

>[!NOTE]
>
>Active profiles are counted based on dedicated technical workflows which run everyday on your instances:
>
>* The ["Billing"](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html?lang=en) workflow for Campaign Standard,
>* The ["Number of active billing profiles"](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/advanced-management/about-technical-workflows.html) workflow for Campaign Classic.

The lower area provides a graphical representation of active profiles usage over the last 30 days. You can change the displayed period of time to 1 year using the available filters in the upper-right corner.

Hovering over one of the graph bars allows you to get the exact number of Active profiles used on the selected period.
