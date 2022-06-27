---
product: campaign
solution: Campaign 
title: SFTP storage management
description: Learn how to monitor and manage your SFTP server's storage
feature: Control Panel
role: Architect
level: Experienced
exl-id: eaf67573-f088-47d9-8a25-273d08dc541a
---
# SFTP storage management {#sftp-storage-management}

>[!CONTEXTUALHELP]
>id="cp_storage"
>title="About storage capacity"
>abstract="In this tab, you can view the storage capacity and utilization information for your SFTP servers. You can also list the top 10 files that are consuming the most space on an SFTP server by clicking its name. Only SFTP servers that you have access to are shown here. Please contact your Administrator to request access to other SFTP servers."
>additional-url="https://images-tv.adobe.com/mpcv3/8a977e03-d76c-44d3-853c-95d0b799c870_1560205338.1920x1080at3000_h264.mp4" text="Watch demo video"

You may have different storage capacity provisioned on your SFTP server, depending on your contractual terms.

It is essential that you regularly monitor available space for each of your SFTP servers. Otherwise, you may not be able to save any additional files on the server anymore, or to successfully execute workflows that rely on the updates from this server.

![](assets/do-not-localize/how-to-video.png) Discover this feature in video using [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/sftp-management/monitoring-server-capacity.html#sftp-management) or [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/sftp-management/monitoring-server-capacity.html#sftp-management)

## Accessing storage capacity information {#accessing-storage-capacity-information}

Information about the space used by all instances you have access to is available in the **[!UICONTROL Storage]** tab of the SFTP card. It is updated on each page refresh.

![](assets/control_panel_space.png)

For each instance, a visual alert lets you know when its storage surpasses its capacity:

* **Orange**: the instance surpassed 80% of its capacity,
* **Red**: the instance surpasses 90% of its capacity.

You can also identify the top 10 files that are consuming the most space on an SFTP server by clicking its name.

![](assets/sftp-top10.png)

Additional tips are also available to help you know how to proceed as your server approaches its capacity.

## Best practices when the storage capacity runs out {#best-practices-when-capacity-runs-out}

1. **Clean the SFTP server from old or unnecessary files**. For more on how to access your SFTP server folder, refer to [this section](../../sftp/using/logging-into-sftp-server.md).
1. Ensure that the **workflows** that clean your SFTP servers are successfully executing. For more on technical workflows in Adobe Campaign, refer to the dedicated [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/advanced-management/about-technical-workflows.html) and [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html) documentations.
1. Reach out to your account team to **request more storage** (additional charges may apply).
1. Reach out to **Customer Care** if you believe there is an issue.
