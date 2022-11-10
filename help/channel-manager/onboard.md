---
title: Onboard [!DNL Channel Manager]
description: 'Connect your instance to the [!DNL Channel Manager] service by completing a few onboarding steps.'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
---

# Onboard [!DNL Channel Manager]

After you complete the Channel Manager onboarding process, you can access, configure, and manage Walmart Marketplace channel sales operations from Adobe Commerce. Channel Manager is available from the [!UICONTROL Channel Manager] option on the [!UICONTROL Commerce Admin Marketing] menu.

![[!DNL Channel Manager] option in Admin view](assets/channel-manager-admin-view.png)

## Requirements

Review the requirements for using Channel Manager and gather the required account information and credentials to download, install, and configure the extension. 

-  **[Walmart Marketplace requirements](walmart-requirements.md)**–Verify that you meet the requirements to integrate with Channel Manager including [setting up your Seller account](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) and generating the API key to enable the integration.

- **Commerce account information**–Downloading and installing [!DNL Channel Manager] requires a [Commerce account](https://docs.magento.com/user-guide/magento/magento-account.html){target="_blank"}. You need an account ID and credentials with Owner or Admin access to the [!DNL Adobe Commerce] or [!DNL Magento Open Source] instance.

  - **MAGE ID**–[Log in](https://account.magento.com/customer/account/login/) to the [!DNL Commerce] account to get the ID from **[!UICONTROL My Account - Magento settings]**.

     ![[!DNL MAGEID] on [!DNL Commerce] account settings](assets/mageid-my-commerce-account.png) 

  - **Access keys–** Get authentication keys to download [!DNL Commerce] extensions from the [!DNL Commerce] Composer repository `([!DNL repo.magento.com]`).

    ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

    On Adobe Commerce and Magento Open Source projects, the owner can set up [Shared Access](https://docs.magento.com/user-guide/magento/magento-account-share.html) to allow trusted employees and service providers to download extensions using credentials from the Owner or license holder account.

    For [!DNL Adobe Commerce] on cloud infrastructure projects, software installers must have the following access to the [!DNL Commerce] instance:

    - Super User access to the Cloud project
    - Admin access to a specific environment
    - an [!DNL Adobe Commerce] account with permissions to access the Composer repository
    
    See [Manage user access](https://devdocs.magento.com/cloud/project/user-admin.html).

- **Experience using Composer and the [!DNL Commerce CLI]**–See [General CLI Installation](https://devdocs.magento.com/extensions/install/){target="_blank"} for information about using these tools to install and manage extensions on [!DNL Adobe Commerce] or [!DNL Magento Open Source] platforms.

- **[[!DNL Amazon Sales Channel] version 4.4.2 or later](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**–If you activated [!DNL Amazon Sales Channel] for your [!DNL Commerce] sites, verify that your [!DNL Commerce] platform has version 4.4.2 or later installed before you install [!DNL Channel Manager].

- **[!DNL Inventory Management] extension for Adobe Commerce and Magento Open Source**

   If you plan to use Channel Manager for inventory and order management, you must have the Inventory Management extension installed and enabled on your Adobe Commerce and Magento Open Source instance. Typically, this extension is installed and enabled by default on Adobe Commerce and [!DNL Magento Open Source] 2.3.x and later.
   
   If you upgraded Commerce from 2.2.x, or if you have disabled Inventory Management, update your installation to include the required modules. See [Install Inventory Management](https://devdocs.magento.com/extensions/inventory-management/) in the Adobe Commerce Developer documentation.

### System Requirements

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x or later](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] version 4.4.2 or later](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)–If you have activated [!DNL Amazon Sales Channel] for your [!DNL Commerce] sites, verify that your [!DNL Commerce] platform has version 4.4.2 installed before you install [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/) 

### Supported platforms

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce on premises (EE) : 2.4.x
- Magento Open Source 2.4.x

## Onboarding steps

1. [Set up your Walmart Seller account](https://seller.walmart.com/signup?q=&origin=solution_provider&src=0014M00001zivMp).

1. [Install the [!DNL Channel Manager] extension](install.md).

1. [Connect to Commerce Services](connect.md) to integrate Channel Manager with the Commerce instance, and other supporting services.

1. [Connect your [!DNL Commerce] store to [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Complete store setup](complete-sales-channel-store-setup.md).
