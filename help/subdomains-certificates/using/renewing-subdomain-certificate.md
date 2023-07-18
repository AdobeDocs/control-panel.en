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
# Renew SSL certificates {#renewing-subdomains-ssl-certificates}

>[!CONTEXTUALHELP]
>id="cp_add_ssl_certificate"
>title="SSL certificate renewal"
>abstract="To renew an SSL certificate, you need to generate a CSR, purchase the SSL certificate for your subdomains, and install the Certificate Bundle."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#generating-csr" text="Generating a Certificate Signing Request (CSR)"

The SSL certificate renewal process includes 3 steps:

1. **Generation of the Certificate Signing Request (CSR)**
    
    Certificate Signing Request has to be generated for the instance and subdomains you are planning to secure prior to purchasing a certificate.  You will need to provide some information required to generate the CSR (such as Common Name, Organization Name and address, etc.). [Learn more](#generate)

1. **Purchase of the SSL certificate**
    
    Once the CSR is generated, you can use it to purchase the SSL certificate from the Certificate Authority that your company approves.

1. **Installation of the SSL certificate**
    
    Install the purchased SSL certificate on the desired subdomain to secure them. [Learn more](#install)

![](assets/do-not-localize/how-to-video.png) Discover this feature in video using [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/subdomains-and-certificates/adding-ssl-certificates.html#subdomains-and-certificates) or [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/subdomains-and-certificates/adding-ssl-certificates.html#adding-ssl-certificates)

**Related topics:**

* [Deliverability Best Practice Guide - SSL certificate request process for Adobe Campaign](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-ssl-certificate-request.html)
* [Subdomains branding](../../subdomains-certificates/using/subdomains-branding.md)
* [Monitoring your subdomains](../../subdomains-certificates/using/monitoring-subdomains.md)

## Generate the CSR {#generate}

>[!CONTEXTUALHELP]
>id="cp_generate_csr"
>title="CSR generation"
>abstract="Certificate Signing Request has to be generated for the instance and subdomains you are planning to secure prior to purchasing a certificate."

>[!CONTEXTUALHELP]
>id="cp_select_subdomains"
>title="Select the subdomains for your CSR"
>abstract="You can choose to include all or only specific subdomains into your Certificate Signing Request. Only selected subdomains will be certified through purchased SSL certificate."

To generate a Certificate Signing Request (CSR), follow these steps:

1. In the **[!UICONTROL Subdomains & Certificates]** card, select the desired instance, then click the **[!UICONTROL Manage Certificate]** button.

    ![](assets/renewal1.png)

1. Select **[!UICONTROL 1 - Generate a CSR]**, then click **[!UICONTROL Next]** to launch the wizard that will guide you through the CSR generation process.

    ![](assets/renewal2.png)

1. A form displays, with all the details required to generate your CSR.

    Make sure you fill in the requested information fully and accurately, otherwise the certificate may not be renewed (contact your internal team, Security and IT teams if necessary), then click **[!UICONTROL Next]**.

    * **[!UICONTROL Organization]**: official organization name.
    * **[!UICONTROL Organization Unit]**: unit linked to the subdomain (example: Marketing, IT).
    * **[!UICONTROL Instance]** (pre-filled): URL of the Campaign instance associated to the subdomain.
    * **[!UICONTROL Common name]**: the common name is selected by default, you can select one of the subdomains if necessary.

    ![](assets/renewal3.png)

1. Select the subdomains to include into the CSR, then click **[!UICONTROL OK]**.

    ![](assets/renewal4.png)

1. The selected subdomains display in the list. For each of them, select the subdomains to include, then click **[!UICONTROL Next]**.

    ![](assets/renewal5.png)

1. A summary of the subdomains to include in the CSR displays. Click **[!UICONTROL Submit]** to confirm your request.

    ![](assets/renewal6.png)

    >[!NOTE]
    >
    >The **[!UICONTROL Copy CSR content]** button allows you to copy all information related to the CSR (Org ID, instance, organization name, common name, included subdomains etc.)

1. The .csr file corresponding to your selection is automatically generated and downloaded. You can now use it to purchase the SSL certificate from the Certificate Authority that your company approves. If you need to download CSR again, follow the steps detailed in [this section](#download).

Once your CSR has been generated and downloaded, you can use it to purchase an SSL certificate from a Certificate Authority approved by your organization.

After the SSL certificate has been purchased, you will be able to install it on your instance to secure your subdomain. [Learn more](install-ssl-certificate.md)

## Download the CSR {#download}

In order to purchase an SSL certificate, you first need to download the Certificate Signing Request. CSR is automatically downloaded after it has been generated. You can also download it again at any time from the Job Logs:

1. In the **[!UICONTROL Job Logs]**, select the **[!UICONTROL Finished]** tab, then filter the list in order to display jobs related to subdomains management.

    ![](assets/renewal-download.png)

1. Open the job corresponding to the generation of the CSR, then click the **[!UICONTROL Downbload]** link to get the .csr file.

    ![](assets/renewal-download-button.png)

## Install the SSL certificate {#install}

>[!CONTEXTUALHELP]
>id="cp_install_ssl_certificate"
>title="SSL Certificate installation"
>abstract="Install the SSL Certificate that you purchased from the Certificate Authority approved by your organization."

Once an SSL certificate has been purchased, you can install it on your instance. Before proceeding, make sure you are aware of the prerequisites below:

* The Certificate Signing Request (CSR) must have been generated from the Control Panel. Otherwise, you will not be able to install the certificate from the Control Panel.
* The certificate Signing Request (CSR) should match the subdomain that has been configured to work with Adobe. For example, it cannot contain more subdomains than the one that has been configured.
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
