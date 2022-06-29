---
product: campaign
solution: Campaign 
title: Renewing a subdomain's SSL certificate
description: Learn how to renew your subdomains' SSL certificates
feature: Control Panel
role: Architect
level: Experienced
---
# Install the SSL certificate {#installing-ssl-certificate}

>[!CONTEXTUALHELP]
>id="cp_install_ssl_certificate"
>title="SSL Certificate installation"
>abstract="Install the SSL Certificate that you purchased from the Certificate Authority approved by your organization."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html" text="About subdomains branding"

Once an SSL certificate has been purchased, you can install it on your instance. Before proceeding, make sure you are aware of the prerequisites below:

* The Certificate Signing Request (CSR) must have been generated from the Control Panel. Otherwise, you will not be able to install the certificate from the Control Panel.
* The certificate Signing Request (CSR) should match the subdomain that has been configured to work with Adobe. For example, it cannot contain more subdomains that the one that has been configured.
* The certificate should have a current date. It is not possible to install certificates with dates in the future, and should not be expired (i.e. valid start and end dates).
* The certificate should be issued by a trusted certificate authority (CA) such as Comodo, DigiCert, GoDaddy, etc.
* The size of the certificate should be 2048 bits and the algorithm should be RSA.
* The certificate should be in X.509 PEM format.
* SAN certificates are supported.
* Wildcard certificates are not supported.
* The ZIP file or the certificate should not be password protected.
* The ZIP file should only contain the following in preferably individual files:
    * End-Entity Certificate.
    * Intermediate Certificate Chain (arranged in proper order).
    * Root certificate (Optional).

To install the certificate, follow these steps:

1. In the **[!UICONTROL Subdomains & Certificates]** card, select the desired instance, then click the **[!UICONTROL Manage Certificate]** button.

    ![](assets/renewal1.png)

1. Select **[!UICONTROL 3 - Install Certificate Bundle]**, then click **[!UICONTROL Next]** to launch the wizard that will guide you through the certificate installation process.

    ![](assets/install1.png)

1. Select the .zip file that contains the certificate to install, then click **[!UICONTROL Submit]**.

    ![](assets/install2.png)

>[!NOTE]
>
>The certificate will get installed on all domains/subdomains included in the CSR. Any additional domain/subdomain present in the certificate will not be taken into account.

Once the SSL certificate is installed, the certificate's expiration date and status icon are updated accordingly.

**Related topics:**

* [Subdomains branding](../../subdomains-certificates/using/subdomains-branding.md)
* [Monitoring your subdomains](../../subdomains-certificates/using/monitoring-subdomains.md)
