---
product: campaign
solution: Campaign 
title: Email alerting
description: Learn how to receive email notifications in case of issues with your Campaign instances
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: 7942d2b1-d28f-4760-aa25-5ba94a627fd0
---
# Email alerting {#email-alerting}

In order to provide greater flexibility to your work, Control Panel is equipped with real-time email alerting functionality.

## List of alerts {#list}

The list of alerts is as follows:

* **SFTP storage usage**: One of your SFTP servers has reached 80% or more of its capacity. See [SFTP storage management](../../sftp/using/sftp-storage-management.md).

* **Database usage**: One of your instances' databases has reached 80% or more of its capacity. See [Database monitoring](../../performance-monitoring/using/database-monitoring.md).

* **SFTP IP allow listing expiration**: One of the IP ranges you defined has expired or is going to expire in 10 days or less. See [IP range allow listing](../../sftp/using/ip-range-allow-listing.md).

* **SFTP public key expiration**: One of the public keys you defined has expired or is going to expire in 10 days or less. See [Key management](../../sftp/using/key-management.md).

* **SSL certificate expiration**: One of your subdomains' SSL certificates has expired or is going to expire in  30 days or less. See [Monitoring subdomains' SSL certificates](../../subdomains-certificates/using/monitoring-ssl-certificates.md).

<!--* **Long running Queries**: A query has been running for more than 24 hours on one of your instances. See [Monitoring active queries](database-active-queries.md).-->

>[!NOTE]
>
>Additionally, Control Panel allows you to **set reminders** in order to be notified by email before an event is going to occur on your instances (releases and service reviews).
>
>To do this, you need to have subscribed to email alerts and set a reminder for the desired upcoming events. [Learn how to set reminders for upcoming events](../../service-events/service-events.md#reminders)

## Subscribe to alerts {#subscribe}

To subscribe to these alerts, follow these steps:

1. Click the **[!UICONTROL Alerting notifications]** button available from any location in the Control Panel, then click **[!UICONTROL Subscribe]**.

    ![](assets/subscribing.png)

1. An email is sent to confirm your subscription.

    ![](assets/email_subscription.png)

1. After subscribing, Control Panel will notify about system issues and recommend the actions to take. Email alerts are sent to everyone who has signed up for **all instances** that they are Administrators of.

    ![](assets/alert_sample.png)
