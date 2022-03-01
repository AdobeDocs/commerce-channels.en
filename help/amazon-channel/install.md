---
title: Install the extension
description: To integrate your [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] and sell through the [!DNL Amazon Marketplace], download and install the Amazon Sales Channel extension.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
---
# Install the extension

>[!IMPORTANT]
>
>Only [!DNL Amazon Sales Channel] extension 4.0+ versions are supported for Adobe Commerce and Magento Open Source 2.4.x versions. If you are running a 2.3.x version, refer to the documentation for the [compatible Amazon sales channel release](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target="_blank"}. For more information about version compatibility, see the [Availability](https://devdocs.magento.com/release/availability.html){target="_blank"} page in the developer documentation.

The [!UICONTROL Amazon Sales Channel] extension installs and adds features to integrate your Commerce catalog with [!DNL Amazon Seller Accounts] to sell through the [!DNL Amazon Marketplace]. To review additional information, see the [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) page in [!DNL Commerce Marketplace] and the [release notes](release-notes.md).

## Requirements

-  **Commerce instance**: The [!DNL Amazon Sales Channel] extension can be installed on instances with Magento Open Source, Adobe Commerce, and Adobe Commerce on cloud infrastructure versions 2.3.x or later. It is no longer supported on 2.1, 2.2, or 1.x releases.
-  **Commerce web account**: You should have a Commerce web account, which is used to create and track an API key.
-  **API key**: Create an Amazon sales channel API key through your Commerce web account. The following instructions include these steps.

## Install

For more detailed information about using Composer for this process, see the [extension installation](https://devdocs.magento.com/extensions/install/){target="_blank"} instructions in the developer documentation.

1. Log in to the [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. Click the **[!UICONTROL Marketplace]** tab, and then click **[!UICONTROL My Purchases]**.

1. Locate and select **[!UICONTROL Amazon Sales Channel]**.

1. On the extension page, select the version.

1. For the component name and version, click **[!UICONTROL Technical Details]**.

1. Use the name and version information to update the services connector entry in your `composer.json` file.

   -  Add the extension's name and version to your `composer.json` file.

   -  Navigate to your [!DNL Commerce] project directory and update your `composer.json` file.

     ```bash
     composer require magento/services-connector:~1.0.3
     ```

   -  Enter your [authentication keys](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"}. Your public key is your username; your private key is your password.

   -  Wait for Composer to finish updating your project dependencies and ensure that there are no errors.

1. [Verify the extension](https://devdocs.magento.com/extensions/install/#verify-the-extension){target="_blank"}.

## Add the Amazon sales channel API key

After installing, enter an [API Key](./amazon-verify-api-key.md) to complete configuration.

## Set the Amazon channel configuration options

You have the following options for configuring the Amazon sales channel. You do not need to modify these settings to begin onboarding and selling on Amazon. It is recommended that advanced administrators consider these options.

1. Log into the Admin.

1. On the _Admin_ sidebar, go to **Stores** > _Settings_ > **Configuration**.

1. Click **Sales Channels**, then **Global Settings**.

1. For **Clear Log History**, define the interval for clearing the collected logs.

   Options include `Once Daily`, `Once Weekly`, and `Once Monthly` (default).

1. (Optional) For **Background Tasks (CRON) Source**, change the setting to `Command Line (CLI) CRON`.
   
   This setting is recommended for **_advanced users/administrators_**. 

1. Click **[!UICONTROL Save Config]**.

## Update the extension

1. Log in to the [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. Click the **[!UICONTROL Marketplace]** tab, and then click **[!UICONTROL My Purchases]**.

1. Locate and select **[!UICONTROL Amazon Sales Channel]**.

1. On the extension page, select the version.

1. For the component name and version, click **[!UICONTROL Technical Details]**.

1. Complete the [extension upgrade instructions](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target="_blank"} in the developer documentation.
