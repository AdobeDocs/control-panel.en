---
product: campaign
solution: Campaign 
title: Add a BIMI record for a subdomain
description: Learn how to add a BIMI record for a subdomain.
feature: Control Panel
role: Architect
level: Experienced
---

# Add a BIMI record for a subdomain {#dmarc}

BIMI: Brandin Indicators for Message Identification
Brand Indicators for Message Identification (BIMI) is an industry standard that allows an approved logo to appear next to a sender’s email in participating platforms.
With this standard, a brand can determine a logo which should be displayed in mailbox providers’ inboxes. Once published in a so-called BIMI DNS (Domain Name System) record, a mailbox provider might pick this logo up and display it in the inbox if certain criteria are met. It can help build more trust with your recipients and therefore drive more engagement though.

Deliverability best practice guide
https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/technotes/implement-bimi.html?lang=en






Limitations/prerequisites
SPF, DKIM and DMARC records are prerequisites for creating BIMI record
only support NS type subdomain
each subdomain can have only 1 BIMI




Add BIMI record
- … / subdomain details / Add TXT record
- Check subdomain name correct
- Record type:  BIMI
- company logo url: secured URL for saved SVG image. 
- Certificate URL
- Click Add. 	if dMarc policy selected as none: cannot create 
- Wait for job to complete

	link to svg file.
certificate: optional. If working as nike.com. cannot download the logo for google. Also add a certificat url repenses the fact that we own this logo. Ownership. Say can put in the certificate link to prove their ownership. Add steps