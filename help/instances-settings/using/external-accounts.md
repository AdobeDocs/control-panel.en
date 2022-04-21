---
product: campaign
solution: Campaign 
title: Connect hybrid instances
description: Learn how to connect instances with an hybrid hosting model to Control Panel
feature: Control Panel
role: Architect
level: Intermediate
---

# Connect hybrid instances

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_url"
>title="Subdomain details"
>abstract="In this screen, you can connect a hybrid instance to the Control Panel in order to monitor it and perform specific actions directly from the Control Panel interface."

Control Panel allows you to connect hybrid instances in order to monitor them and perform specific actions [listed here](#capabilities) directly from the Control Panel interface. For more information on  hosting models, refer to [Campaign Classic documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/architecture-and-hosting-models/hosting-models-lp/hosting-models.html).

## Connect an hybrid instance {#connect}

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_operator"
>title="Subdomain details"
>abstract="ID of the operator used in the Client Console to add the MID/RT instance in the marketing instance."

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_password"
>title="Subdomain details"
>abstract="Password of the operator used in the Client Console to add the MID/RT instance in the marketing instance."

To connect an hybrid instance to the Control Panel, follow these steps:

1. In the **[!UICONTROL Instances Settings]** card, select the **[!UICONTROL External Accounts]** tab.

1. Select the MID/RT instance to connect to your hybrid instance, then click **[!UICONTROL Add new URL]**.

    ![](assets/external-account-addbutton.png)

1. Provide information about the hybrid instance to connect:

    * **[!UICONTROL URL]**: URL of the instance,
    * **[!UICONTROL Operator]** / **[!UICONTROL Password]**: Credentials of the operator used in the Client Console to add the MID/RT instance in the marketing instance.

    ![](assets/external-account-add.png)

1. Click **[!UICONTROL Save]** to confirm.

Your instance is now connected to the Control Panel. You can remove or deactivate a connection at any time by selecting it from the list.

![](assets/external-account-edit.png)

## Capabilities available to hybrid instances {#capabilities}

Once an hybrid instance is connected to the Control Panel, you can leverage the Control Panel capabilities listed below to monitor it:

* [Delegate subdomains](../../subdomains-certificates/using/setting-up-new-subdomain.md)
* [View your instance details](../../instances-settings/using/instance-details.md)
* [Add IP addresses to the allow list to access your instances](../../instances-settings/using/ip-allow-listing-instance-access.md)
* [Monitor and install SSL certificates](../../subdomains-certificates/using/monitoring-ssl-certificates.md)
