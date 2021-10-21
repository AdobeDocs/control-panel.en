---
product: campaign
solution: Campaign 
title: Control Panel FAQ
description: Common questions related to the Control Panel
feature: Control Panel
role: Architect
level: Intermediate
exl-id: 4f329764-ed8b-4939-affc-ed994fd6101d
---
# Frequently Asked Questions {#faq}

## Control Panel {#control-panel}

### What is the Control Panel?

The Control Panel empowers product admins to directly manage various settings and monitor capacity of SFTP servers connected to Adobe Campaign.

### What are some of the current capabilities of the Control Panel?

Control Panel allows you to track storage, add IPs to the allow list, and manage SSH keys for your SFTP servers on your own based on your needs, and other actions.

For more information, refer to the Control Panel supported actions documentation.

### Which capabilities are not supported on Campaign v8 but available on Campaign Classic v7{#v8-restrictions}

Sub-Domain and Certificate Management related functions are not yet supported through Control Panel on Campaign v8. Contact Campaign Customer Care for any related support.

### Is the Control Panel only for Adobe Campaign?

Yes, you will only be able to manage settings for Adobe Campaign in the Control Panel.

### Can I use the Control Panel?

The Control Panel is only open to product admins of our current customers who have Adobe Campaign hosted on AWS. Note that hybrid environments are not yet supported.

If you're not an admin, but would like access, please contact your product admin to help add you as an admin.

### As a Campaign Classic v7 user, what are the conditions to access Control Panel? {#v7-restrictions}

Control Panel is restricted to Admin users. [Learn more](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html#discover-control-panel).

For Campaign Classic v7, note that your instance must be hosted on Amazon Web Services (AWS) and upgraded to the latest [Campaign GA](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/rn-overview.html#rn-statuses) build. Learn how to check your Campaign Classic version in [this section](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html#getting-your-campaign-version). To check if your Campaign Classic instance is hosted on AWS, follow the steps detailed in [this section](#hosted-aws).

### How can I access the Control Panel?

Please follow the detailed instructions in the Accessing the Control Panel documentation.

### Is there an extra fee to use the Control Panel?

No, there is no extra cost if you are a current customer of Adobe Campaign.

## IMS Organization ID {#ims-org-id}

### What is an IMS Organization ID?

It is a unique ID that is given to your instance when you first log onto Adobe Experience Cloud. It should be in the format: xxx@AdobeOrg.

For more information, please refer to [Adobe Experience Cloud documentation](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html).

### Where can I find my IMS Organization ID?

One way is to navigate to [Adobe Experience Cloud Home](https://experiencecloud.adobe.com/) > **[!UICONTROL Administration]**. You will find your IMS Organization ID at the bottom of Administration **[!UICONTROL Quick Access]** section. You can find more detailed information in the [Adobe Experience Cloud documentation](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html).

The other way is to launch **Admin Console**. Your IMS Organization ID will be visible in your URL, it should look something like: https://adminconsole.adobe.com/xxx@AdobeOrg/overview.

### Why do I need to know my IMS Organization ID?

In order for you to manage settings for your instance, we want to ensure that you're getting the right information for the right instance in case you're using multiple instances for your company.

### What if I have multiple IMS Organization IDs?

You may have more than one IMS Organization ID if you have access to multiple Adobe solutions. In this case, the correct IMS Organization ID you should be using is the one you see under your Adobe Campaign instance.

>[!NOTE]
>
>If you have the same IMS Organization ID for Adobe Campaign and Adobe Analytics, this is great. Having one IMS Organization ID between Analytics and Campaign is a requirement if you plan to integrate the solutions to take advantage of complex use cases such as shopping cart abandonment (for AA + AC).
>
>If you have different IMS Organization IDs for Adobe Campaign and Adobe Analytics, please reach out to Customer Care to get them aligned.

### How can I know that my Adobe Campaign instance is hosted on AWS or not?{#hosted-aws}

To check if your instance is hosted on AWS, follow these steps:

1. Retrieve your login URL. It is the URL that you use to login to your Campaign instance, it mostly ends with ".campaign.adobe.com" or“.neolane.net”.
1. Open the terminal, then execute a **[!DNL nslookup]** operation on your login URL.

    `doe-macOS% nslookup myinstance.campaign.adobe.com`

1. The response returns information on your instance.

    ```

    doe-macOS% nslookup myinstance.campaign.adobe.com
    Server:     12.34.5.678
    Address:    12.34.5.678#99
  
    Non-authoritative answer:
    myinstance.campaign.adobe.com
    canonical name = myinstance-mkt-prod1.campaign.adobe.com.
    myinstance-mkt-prod1.campaign.adobe.com
    canonical name = myinstance-mkt-prod1-1.campaign.adobe.com.
    Name: myinstance-mkt-prod1-1.campaign.adobe.com
    Address: 12.34.567.89

    ```

1. Execute a **nslookup** operation on the returned IP address.

    `doe-macOS% nslookup 12.34.567.89`

1. Check the "name" value in the returned result. If it contains "amazonaws.com", this means your instance is hosted on AWS.

    ```

    doe-macOS% nslookup 12.34.567.89
    Server:     12.34.5.678
    Address:    12.34.5.678#99

    Non-authoritative answer:
    89.567.34.12.in-addr.arpa   name = ec2-12-34-567-89.address.amazonaws.com.

    ```

>[!NOTE]
>
>If you would like to be migrated to AWS, please start the process by contacting your Customer Success Manager.
