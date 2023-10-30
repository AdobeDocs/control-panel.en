---
product: campaign
solution: Campaign 
title: Instance details
description: Learn how to monitor your instance details in the Control Panel
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: 02819bfc-9886-43fc-8014-9bfe64c42048
---
# Instance details {#instance-details}

>[!CONTEXTUALHELP]
>id="cp_instancesettings_instancedetails"
>title="About Instance details"
>abstract="View the details of your Adobe Campaign instances: types, names, build information, and possible upgrade recommendations."

## About instance details {#about-instance-details}

>[!IMPORTANT]
>
>This feature is available for Campaign v7/v8 instances only.

Your Adobe Campaign instance architecture can contain several servers to enable the flexibility of marketing activities. For example, you can have Marketing, Real Time (or Message Center) and Mid Sourcing servers supporting your instance. 

The Instance Details functionality allows you to view flat architecture of your instance. In addition to server information, it also lets you know whether or not your instance build is current, as well as recommends upgrades when needed. 

>[!NOTE]
>
>We recommend that your instances are upgraded at least once a year in order to avoid performance degradation, and be able to take the advantage of the newest features and fixes Adobe Campaign v7/v8 has to offer.

**Related topics:**

* [Performing a build upgrade](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/updating-adobe-campaign/build-upgrade.html)
* [Updating Adobe Campaign](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/updating-adobe-campaign/introduction.html)

## Retrieving information about your instances {#retrieving-information-about-instances}

To get information on the servers connected to your instances, follow these steps:

1. Open the **[!UICONTROL Instances Settings]** card to access the **[!UICONTROL Instance Details]** tab.

    >[!NOTE]
    >
    >If the Instance Settings card is not visible on the homepage of the Control Panel, this means your organization ID is not associated with any Adobe Campaign v7/v8 instances

1. Select in the left pane the desired Campaign instance.

    >[!NOTE]
    >
    >All your Campaign instances display in the left pane list. As the Instance Details feature is dedicated to Campaign v7/v8 instances only, the "Non-Applicable Instance" message displays if you select a Campaign Standard instance.  

1. The servers connected to the instance display.

   ![](assets/instance_details.png)

Available information are:

* **[!UICONTROL Type]**: the type of the server. Possible values are MKT (Marketing), MID (Mid sourcing), and RT (Message Center / Real-time messaging).
* **[!UICONTROL Name]**: the name of the server.
* **[!UICONTROL Build:]** the build version installed on the server.
* **[!UICONTROL Upgrade info]**: this column informs you if any update is required for the server.
    * Green: your server is current, no upgrade is required.
    * Yellow: you should consider upgrading. You are missing the newest features and fixes.
    * Red: upgrade as soon as possible. You are missing new features and the server performance might not be optimal.

If one of your servers requires to be upgraded, refer to [this documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/updating-adobe-campaign/build-upgrade.html) for more details on how to proceed.

## Common questions {#common-questions}

**I do not see the MID server on my instance architecture, does it mean my instances are not functioning correctly? Do I need the RT instance for something I am not able to do today?**

Your own instance can look very different, and it may not have all types of servers, or it can have several of the same server. Not having one type of the server or another does not mean you cannot send a real-time message or perform other kinds of activities. You can request additional server capacity, additional fees will apply.

Please contact Customer Care if you believe some servers are not showing in the "Instance Details" page. Make sure you note the specific instance URL in your message.
