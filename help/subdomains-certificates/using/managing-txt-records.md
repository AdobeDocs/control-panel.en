---
product: campaign
solution: Campaign 
title: Add a Google TXT record for a subdomain
description: Learn how to add a Google TXT record for a subdomain for domain ownership verification.
feature: Control Panel
role: Architect
level: Experienced
exl-id: 547ca6f2-720f-4d58-b31b-5b2611ba9156
---
# Add a Google TXT record {#adding-a-google-txt-record}

To add a Google TXT record to your subdomain used to email Gmail addresses, follow these steps:

1. Navigate to the **[!UICONTROL Subdomain and Certificates]** card.

1. Select your instance, then open the details of the subdomain to which you would like to add a DNS record.

    ![](assets/txt_subdomaindetails.png)

1. Click the **[!UICONTROL Add TXT record]** button, then enter the value generated in G Suite Admin tools. For more on this, refer to the [G Suite Admin Help](https://support.google.com/a/answer/183895).

    ![](assets/txt_addtxt.png)

1. Click the **[!UICONTROL Add]** button to confirm.

    ![](assets/txt_txtadded.png)

Once the TXT record is added, you need to have it verified by Google. To do this, navigate to the G Suite Admin tools then launch the verification step (see [G Suite Admin Help](https://support.google.com/a/answer/183895)).

To delete a record, select it from the records list, then click the remove button.

>[!NOTE]
>
>The only record that you can delete from the DNS records list is the one that you have previously added (in our case the Google TXT record).

![](assets/do-not-localize/how-to-video.png) Discover this feature in video using [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/subdomains-and-certificates/google-txt-record-management.html#subdomains-and-certificates) or [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/subdomains-and-certificates/google-txt-record-management.html#subdomains-and-certificates)
