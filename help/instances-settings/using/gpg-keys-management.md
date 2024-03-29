---
product: campaign
solution: Campaign 
title: GPG keys management
description: Learn how to manage GPG keys to encrypt and decrypt data within Adobe Campaign.
feature: Control Panel, Encryption
role: Admin
level: Experienced
exl-id: 366dd2ea-c6be-41a2-a4d6-4ffecb5f3d39
---
# GPG keys management {#gpg-keys-management}

>[!CONTEXTUALHELP]
>id="cp_instancesettings_gpg_management"
>title="About GPG keys"
>abstract="In this tab, you can install and/or generate GPG keys on a marketing instance, in order to encrypt data sent from Campaign and decrypt incoming data."
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html" text="About performance monitoring"

## About GPG encryption {#about-gpg-encryption}

GPG encryption allows you to protect your data using a system of public-private keys pairs that follow the [OpenPGP](https://www.openpgp.org/about/standard/) specification.

Once implemented, you can have incoming data decrypted and outgoing data encrypted before transfer occurs, to ensure that they will not be accessed by anyone without a valid matching key pair.

To implement GPG encryption with Campaign, GPG keys must be installed and/or generated on a marketing instance by an Administrator user directly from the Control Panel.

You will then be able to:

* **Encrypt sent data**: Adobe Campaign sends data out after encrypting it with the installed public key.

* **Decrypt incoming data**: Adobe Campaign receives data that has been encrypted from an outside system using a public key downloaded from the Control Panel. Adobe Campaign decrypts the data using a private key that is generated from the Control Panel.

## Encrypting data {#encrypting-data}

Control Panel allows you to encrypt data coming out from your Adobe Campaign instance.

To do this, you need to generate a GPG key pair from a PGP encryption tool, then install the public key into Control Panel. You will then be able to encrypt data before sending it from you instance. To do this, follow the steps below.

>[!NOTE]
>
>You can install up to 60 GPG keys in Control Panel.

![](assets/do-not-localize/how-to-video.png) Discover this feature in [video](#video)

1. Generate a public/private key pair using a PGP encryption tool following the [OpenPGP specification](https://www.openpgp.org/about/standard/). To do this, install a GPG utility or GNuGP software.

    >[!NOTE]
    >
    >Open source free software to generate keys is available. However, make sure you follow the guidelines of your organization and use the GPG utility recommended by your IT/Security organization.

1. Once the utility is installed, run the command below, in Mac Terminal or Windows command.

    `gpg --full-generate-key`

1. When prompted, specify the desired parameters for your key. Required parameters are:

    * **key type**: RSA
    * **key length**: 3072 - 4096 bits
    * **real name** and **email address**: Allows to track who created the key pair. Enter a name and email address linked to your organization or department.
    * **comment**: adding a label to the comment field will help you easily identify the key to use to encrypt your data.
        >[!IMPORTANT]
        >
        >Make sure that this field is not left empty and that a comment is filled in.

    * **expiration**: Date or "0" for no expiration date.
    * **passphrase**

    ![](assets/do-not-localize/gpg_command.png)

1. Once confirmed, the script will generate a key with its associated fingerprint, that you can export into a file, or paste directly into the Control Panel. To export the file, run this command followed by the fingerprint of the key that you generated.

    `gpg -a --export <fingerprint>`

1. To install the public key into Control Panel, open the **[!UICONTROL Instance settings]** card, then select the **[!UICONTROL GPG keys]** tab and the desired instance.

1. Click the **[!UICONTROL Install Key]** button.

    ![](assets/gpg_install_button.png)

1. Paste the public key that has been generated from your PGP encryption tool. You can also directly drag and drop the public key file that you exported.

    >[!NOTE]
    >
    >The public key should be in the OpenPGP format.

    ![](assets/gpg_install_paste.png)

1. Click the **[!UICONTROL Install Key]** button.

Once the public key is installed, it displays in the list. You can use the **...** button to download it or copy its fingerprint.

![](assets/gpg_install_download.png)

The key is then available for use in Adobe Campaign workflows. You can use it to encrypt data when using data extraction activities.

![](assets/do-not-localize/how-to-video.png) Discover this feature in [video](#video)

For more on this topic, refer to Adobe Campaign documentation:

**Campaign v7/v8:**

* [Zipping or encrypting a file](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/importing-and-exporting-data/managing-data-encryption-compression/zip-encrypt.html)
* [Use case: Encrypting and exporting data using a key installed on Control Panel](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/importing-and-exporting-data/managing-encrypted-data.html#use-case-gpg-encrypt)

**Campaign Standard:**

* [Managing encrypted data](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/importing-and-exporting-data/managing-encrypted-data.html)
* [Use case: Encrypting and exporting data using a key installed on Control Panel](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/importing-and-exporting-data/managing-data-encryption-compression/zip-encrypt.html#use-case-gpg-encrypt)

## Decrypting data {#decrypting-data}

Control Panel allows you to decrypt external data coming into your Adobe Campaign instances.

To do this, you need to generate a GPG key pair directly from the Control Panel.

* The **public key** will be shared with the external system, which will use it to encrypt the data to send to Campaign.
* The **private key** will be used by Campaign to decrypt the incoming encrypted data.

![](assets/do-not-localize/how-to-video.png) Discover this feature in [video](#video)

To generate a key pair in Control Panel, follow these steps:

1. Open the **[!UICONTROL Instance settings]** card, then select the **[!UICONTROL GPG keys]** tab and the desired Adobe Campaign instance.

1. Click the **[!UICONTROL Generate Key]** button.

    ![](assets/gpg_generate.png)

1. Specify the name of the key, then click **[!UICONTROL Generate Key]**. This name will help you identify the key to use for decryption in Campaign workflows

    ![](assets/gpg_generate_name.png)

Once the key pair is generated, the public key displays in the list. Note that decryption key pairs are generated with no expiration date.

You can use the **...** button to download the public key or copy its fingerprint.

![](assets/gpg_generate_list.png)

The pubic key is then available to be shared with any external system. Adobe Campaign will be able to use the private key in data loading activities to decrypt data that has been encrypted with the public key.

For more on this, refer to Adobe Campaign documentation:

**Campaign v7 and v8:**

* [Unzipping or decrypting a file before processing](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/importing-and-exporting-data/managing-data-encryption-compression/unzip-decrypt.html)
* [Use case: Importing data encrypted using a key generated by Control Panel](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/importing-and-exporting-data/managing-data-encryption-compression/unzip-decrypt.html#use-case-gpg-decrypt)

**Campaign Standard:**

* [Managing encrypted data](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/importing-and-exporting-data/managing-encrypted-data.html)
* [Use case: Importing data encrypted using a key generated by Control Panel](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/importing-and-exporting-data/managing-encrypted-data.html#use-case-gpg-decrypt)

## Monitoring GPG keys

To access GPG keys installed and generated for your instances, open the **[!UICONTROL Instance settings]** card, then select the **[!UICONTROL GPG keys]** tab.

![](assets/gpg_list.png)

The list displays all encryption and decryption GPG keys that have been installed and generated for your instances with detailed information on each key:

* **[!UICONTROL Name]**: The name that has been defined when installing or generating the key.
* **[!UICONTROL Use case]**: This column specifies the key's use case:

    ![](assets/gpg_icon_encrypt.png): The key has been installed for data encryption.

    ![](assets/gpg_icon_decrypt.png): The key has been generated to allow data decryption.

* **[!UICONTROL Fingerprint]**: the fingerprint of the key.
* **[!UICONTROL Expires]**: The key's expiration date. Note that Control Panel will provide visual indications as the key approaches its expiry date:

    * Urgent (red) is shown 30 days before.
    * Warning (yellow) is shown 60 days before.
    * An "Expired" red banner will display once a key expires.

    >[!NOTE]
    >
    >Note that no email notification will be sent by Control Panel.

As a best practice, we recommend that you remove any key that you do not need anymore. To do this, click the **...** button then select **[!UICONTROL Delete Key].**.

![](assets/gpg_delete.png)

>[!IMPORTANT]
>
>Before removing a key, make sure that it is not used in any Adobe Campaign workflow to prevent them from failing.

## Tutorial video {#video}

The video below shows how to generate and install GPG keys for data encryption.

Additional how-to videos related to GPG keys management are available in  [Campaign v7/v8](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/instance-settings/gpg-key-management/gpg-key-management-overview.html#instance-settings) and [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/instance-settings/gpg-key-management/gpg-key-management-overview.html#instance-settings) tutorials pages.

>[!VIDEO](https://video.tv.adobe.com/v/36386?quality=12)
