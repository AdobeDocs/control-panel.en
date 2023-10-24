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
# Monitor active profiles {#active-profiles-monitoring}

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

For more on active profiles, refer to [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/profiles-and-audiences/managing-profiles/active-profiles.html) and [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/profile-management/about-profiles.html#active-profiles) documentations.

## Monitor your active profiles usage {#monitoring-active-profiles}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_active_profile"
>title="About active profiles monitoring"
>abstract="In this tab, you can get real-time information on the latest and historical active profiles usage and evolution for each in your Campaign instances and your organization."

To monitor your active profile usage, navigate to the **[!UICONTROL Performance Monitoring]** card > **[!UICONTROL Active Profiles]** tab, and select the desired instance from the **[!UICONTROL Instance List]**.

Information displays regarding your usage of active profiles. 

![](assets/active-profiles-graph.png)

The upper area displays:
* The number of active profiles used in the selected instance, as well as the last time the billing workflow was run on your instance,
* The number of active profiles used in your organization in all your instances,

    >[!NOTE]
    >
    >This section only displays if you have multiple instances for your organization.

* The number of active profiles your organization is entitled to.

The lower area provides a graphical representation of active profiles usage over the last 30 days. You can change the displayed period of time to 1 year using the available filters in the upper-right corner.

Hovering over one of the graph bars allows you to get the exact number of Active profiles used on the selected period.

>[!NOTE]
>
>Active profiles are counted based on dedicated technical workflows which run everyday on your instances:
>
>* The ["Billing"](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html) workflow for Campaign Standard,
>* The ["Number of active billing profiles"](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/advanced-management/about-technical-workflows.html) workflow for Campaign v7/v8.
