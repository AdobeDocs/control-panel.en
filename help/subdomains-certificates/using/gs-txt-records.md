---
product: campaign
solution: Campaign
title: Managing TXT records
description: Learn how to manage TXT records for domain ownership verification.
feature: Control Panel, Subdomains and Certificates
role: Admin
level: Experienced
exl-id: 013d6674-0988-4553-a23e-b3ec23da5323
TQID: 'https://experienceleague.adobe.com/G8eirPm9hY0XRZTtMOBpmdwxuo3-Uvdo9LQjiSiElPU'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
  - id: a7760dfc-5c44-4d77-bb68-c50b1e265c93
    internal-label: Security and privacy
subfeature_v2:
  - id: f807e46f-d823-43a9-98be-82e0b2f3a05c
    internal-label: Subdomains and certificates
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
---
# Get started TXT records {#managing-txt-records}

>[!CONTEXTUALHELP]
>id="cp_siteverification_add"
>title="Managing TXT records"
>abstract="TXT records are a type of DNS records used to provide text information about a domain, that can be read by external sources. Control Panel allows you to add three types of records to your subdomains: Google Site Verification, DMARC, and BIMI records."

## About TXT records {#about}

TXT records are a type of DNS records used to provide text information about a domain, that can be read by external sources. Control Panel allows you to add three types of records to your subdomains:

* **Google TXT records** allow you to attest that you own your domain, ensuring high inbox rates and low spam rates for your emails. [Learn how to add Google TXT records](managing-txt-records.md)
* **DMARC records** provide a way to authenticate the sender's domain and prevent unauthorized use of the domain for malicious purposes. [Learn how to add DMARC records](dmarc.md)
* **BIMI records** allow you to display an approved logo next to your emails in mailbox providers' inboxes to enhance brand recognition and trust. [Learn how to add BIMI records](bimi.md)

## Monitor your subdomains' records {#monitor}

You can monitor all the TXT records that have been added for each subdomain by accessing the subdomains' details.

In this screen, all the TXT-type records for the selected subdomain display, with information in the "Value" column on their configuration. To delete a Google TXT, DMARC or BIMI record, click the ellipsis button then select Delete. You can also edit DMARC and BIMI records if necessary.

![](assets/txt-records.png)
