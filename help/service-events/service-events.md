---
product: campaign
solution: Campaign
title: Monitor key contacts and events
description: Learn how to identify events occurring on your instances and key contacts at Adobe.
feature: Control Panel
role: Architect
level: Intermediate
exl-id: d230aae6-4f0e-4201-bb3c-0e3f83a7c1b8
---
# Monitor key contacts and events {#keycontacts-events}

>[!CONTEXTUALHELP]
>id="cp_servicecalendar_serviceevents"
>title="Service Calendar"
>abstract="The Key contacts section lists the persons at Adobe to contact for any request or issue on your instances. In the Service Event Calendar section, you can identify past and upcoming releases, alerts for the selected instance and set up reminders for upcoming events."

>[!IMPORTANT]
>
>Service Calendar is available in beta, and subject to frequent updates and modifications without notice.

To effectively monitor your Campaign instances, it is crucial to identify events. The Control Panel allows you to monitor releases and alerts for your instances, and provides a list of key Adobe contacts for any requests or issues.

Identifying events on your Campaign instances is essential to effectively monitor them. Control Panel allows you to monitor releases and alerts for your instances, and provides a list of key Adobe contacts for any requests or issues.

This information is accessible from the **[!UICONTROL Service Calendar]** card on Control Panel homepage.

## Key contacts {#key-contacts}

The **[!UICONTROL Key contacts]** section lists the persons at Adobe that you can contact for any request or issue on your instances.

>[!NOTE]
>
>This section only shows information for Managed Service Accounts.

![](assets/service-events-contacts.png)

Key contacts include the following roles:

* **[!UICONTROL TAM]**: Technical Account Manager,
* **[!UICONTROL CSM]**: Customer Success Manager,
* **[!UICONTROL Deliverability]**: point of contact for deliverability operations,
* **[!UICONTROL Transition Manager]**: Managed Services Transition Manager (Managed Services Account only),
* **[!UICONTROL On-boarding Specialist]**: Specialist assigned to the account to help you on-board onto Campaign Classic (Managed Services Account only).

## Monitor events {#events}

The **[!UICONTROL Service Event Calendar]** section shows all past and upcoming releases, as well as alerts and reminders for the selected instance.

Events are displayed either in a calendar or a list. You can switch between the two views using the **[!UICONTROL Calendar]** and **[!UICONTROL List]** buttons in the upper-right corner of the section.

![](assets/service-events-calendar.png)

<table><tr style="border: 0;">
<td><img src="assets/do-not-localize/nav-buttons.png">
</td><td>In calendar view, navigation buttons are available in the upper-right corner to help you browse across the events. Use the <b>double arrows</b> to navigate to the previous or next event, and the <b>single arrows</b> to navigate from a month to another. Click the <b>circle button</b> to go back to today's view.</td>
</tr></table>

Three types of events are displayed:

* **Reminders** are notifications that can be set to alert users before an event occurs. These are shown in green in the calendar view. [Learn how to set reminder](#reminders)
* **Alerts** are sent via email by the Control Panel to notify users of issues on their instances, such as storage overload or SSL certificate expiration. These are displayed in orange in the calendar view.

    The event description specifies whether the alert is sent to the logged-in user, depending on their subscription to email alerts. [Learn more on Control Panel email alerting capabilities](../performance-monitoring/using/email-alerting.md)

* **Releases** indicate both past and upcoming deployments to the instance, shown respectively in grey and blue in the calendar view.

    The event details specify the type of release associated with each deployment:

    * **[!UICONTROL General availability]**: Latest available stable build.
    * **[!UICONTROL Limited availability]**: On-demand deployment only.
    * **[!UICONTROL Release candidate]**: Engineering validated. Waiting for production proofing.
    * **[!UICONTROL Pre release]**: Earlier availability for specific customer needs.
    * **[!UICONTROL No longer available]**: The build holds no major issue but a new one is available with additional bug fixes. An upgrade is required.
    * **[!UICONTROL Deprecated]**: Build embedding known regressions. The build is no longer supported. An upgrade is mandatory.

Addtionally, you can assign a flag to one or several upcoming events to keep track of them. To do this, hover over the desired event in the calendar or click the ellipse button next to the event name in list view and flag it.

![](assets/service-events-flag.png)

## Set reminders {#reminders}

With Service Calendar, you can set reminders in order to be notified by email before an event is going to occur.

>[!NOTE]
>
>In order to be notified about upcoming events, make sure you have subscribed to email alerts in Control Panel. [Learn more](../performance-monitoring/using/email-alerting.md)

To set an alert for an event, follow these steps:

1. Hover over the event that you want to be reminded of or click the ellipse button in the list view and select **[!UICONTROL Set Reminder]**.

1. Give a title to the reminder and select the date at which you want to be notified before the event occurs.

    ![](assets/service-events-set-reminder.png)

    >[!NOTE]
    >
    >If you have not subscribed to Control Panel alerts, a message will display and allow you to enroll to receive email notifications.

1. The reminder is now set for the selected event. You can hover over it at any time to display its title.

    ![](assets/service-events-reminder.png)

    >[!NOTE]
    >
    >You can set up to 2 reminders for the same event.

1. On the date specified in the reminder, an email will be sent to notify you about the upcoming event, and the reminder will automatically be removed from the **[!UICONTROL Reminders]** count in the Service Calendar menu.
