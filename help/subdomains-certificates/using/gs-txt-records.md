---
product: campaign
solution: Campaign 
title: Managing TXT records
description: Learn how to manage TXT records for domain ownership verification.
feature: Control Panel
role: Architect
level: Experienced
---

# Get started TXT records {#managing-txt-records}

>[!CONTEXTUALHELP]
>id="cp_siteverification_add"
>title="Managing TXT records"
>abstract="Some services like Google require that you add a TXT record to your domain settings in order to verify that you own the domain."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/setting-up-new-subdomain.html" text="Setting up a new subdomain"

TXT records are a type of DNS records used to provide text information about a domain, that can be read by external sources.


list three types of records, why we should add them

To implement this, cp allows to set up two text records:
- BIMI record:logo url + certificate url(?)
- DMARC record: policy to treat failed email




In order to ensure high inbox rates, and low spam rates, some services like Google require that you add a TXT record to your domain settings in order to verify that you own the domain.

Currently, Gmail is among one of the most popular email addresses providers. In order to ensure good deliverability and successful delivery of emails to Gmail addresses, Adobe Campaign allows you to add special Google site verification TXT records to your subdomains to ensure that it is verified.





Edit and delete DMARC/BIMI Record
Access list, … button ?
Voir liste records on peut voir les dim and spf, montrer ?
5 to 7 minutes (add, edit, delete)
