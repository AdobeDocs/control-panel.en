---
product: campaign
solution: Campaign 
title: Add a DMARC record for a subdomain
description: Learn how to add a DMARC record for a subdomain.
feature: Control Panel
role: Architect
level: Experienced
---

# Add a DMARC record for a subdomain {#dmarc}

DMARC (Domain based Message Authentication, Reporting and Conformance) is a standard which allows the brand to decide what a mailbox provider should do with an email which fails authentication. The so-called policies range from “none” over “quarantine” (Spam folder placement) to “reject” (outright block the mail). DMARC  implementation is a requirement for the implementation of BIMI. In addition to DMARC on the sending domain, DMARC also needs to be employed on enforcement level for the organizational domain (if the sending domain is news.example.com, example.com is the organizational domain).

Dmarc based on two records: SPF and DKIM
- Spf based on sender IP whitelisted or not
- Dkim based on authentication, visitor

When email sent from domain, has an IP. Assign it to DKIM value. 
- When received will check wether SPF record and IP from sender match or not. Should match to email IP.
- Should have a DKIM valid



DMARC is an email authentication protocol that helps organizations protect their email domains from phishing and spoofing attacks. It specifies how email receivers should handle messages that fail SPF and DKIM checks, providing a way to authenticate the sender's domain and prevent unauthorized use of the domain for malicious purposes


Limitations/Prerequisites

SPF and DKIM records are prerequisites for creating DMARC record
only support NS type subdomain
each subdomain can have only 1 DMARC


Add DMARC record
- … / subdomain details / Add TXT record
- Check subdomain name correct
- Record type: DMARC
- Policy type: how want mail that fails to be treated by the recipient server: none / quarantine / reject. Recommended first none: 	when setting new domain, possibility you make a mistake. If start rejecting your milans will never find out what went wrong. None: we’re doing nothing when email checks fail. once done, can change
- Email address to receive aggregate-DMARC reports
- Email address to receive forensic DMARC failure reports
    - when check from dcim or spa fails, will get detailed report. Subscribe for daily report. how many email fail. aggreate: High level numbers: how many. Forensic: show detail like from which IPs come from 
- Percentage of email to apply this to (optional). If nothing = 100%
- Reporting interval (optional) in hours. If blank= 24hours. Can put more but not lower. 1 and 2190 (three months)
- SFP identifier alignment . alignment: let’s say sender email is email.adobe.com Spf record is created is aaa.email.nadobe.com
    - If strict > check will fail
    - If relaxed: pass because underlined domain is still the same. 
- Click Add
- Wait for job to complete

