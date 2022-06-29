---
product: campaign
solution: Campaign 
title: Renewing a subdomain's SSL certificate
description: Learn how to renew your subdomains' SSL certificates
feature: Control Panel
role: Architect
level: Experienced
exl-id: e9b7c67d-6afa-44f9-b19d-39c0ec9a7edd
---
# Renewing an SSL certificate {#renewing-subdomains-ssl-certificates}

>[!CONTEXTUALHELP]
>id="cp_add_ssl_certificate"
>title="SSL certificate renewal"
>abstract="To renew an SSL certificate, you need to generate a CSR, purchase the SSL certificate for your subdomains, and install the Certificate Bundle."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#generating-csr" text="Generating a Certificate Signing Request (CSR)"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#installing-ssl-certificate" text="Installing an SSL certificate"

>[!IMPORTANT]
>
>SSL certificate renewal from the Control Panel is available in beta, and subject to frequent updates and modifications without notice.
>
>If you are using an instance with an hybrid hosting model, you can only view certificates associated with the delegated subdomains and will not be able to renew them.

The SSL certificate renewal process includes 3 steps:

1. **Generation of the Certificate Signing Request (CSR)**
    
    Certificate Signing Request has to be generated for the instance and subdomains you are planning to secure prior to purchasing a certificate.  You will need to provide some information required to generate the CSR (such as Common Name, Organization Name and address, etc.). [Learn more](generate-csr.md)

1. **Purchase of the SSL certificate**
    
    Once the CSR is generated, you can use it to purchase the SSL certificate from the Certificate Authority that your company approves.

1. **Installation of the SSL certificate**
    
    Install the purchased SSL certificate on the desired subdomain to secure them. [Learn more](install-ssl-certificate.md)

![](assets/do-not-localize/how-to-video.png) Discover this feature in video using [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/subdomains-and-certificates/adding-ssl-certificates.html#subdomains-and-certificates) or [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/subdomains-and-certificates/adding-ssl-certificates.html#adding-ssl-certificates)
