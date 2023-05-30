---
title: Add or Verify the Amazon API Key
description: In your Commerce configuration, the validated Amazon API key allows you to integrate your stores with your Amazon Seller account.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
---
# Add or Verify the Amazon API Key

When accessing Amazon sales channel, [!DNL Commerce] automatically checks and validates the Amazon API key you have added in your store configuration. If validated, then you can move on to the next step, [Store Integration](./store-integration.md).

If the Amazon API key is missing, invalid, or expired, you must update your key. A message appears prompting you to get an API key and to add they key to your Amazon sales channel configuration.

## Get and add the Amazon API key as prompted

The API key is validated each time you access your Amazon sales channel.

1. Log into the [!DNL Commerce] Admin.

1. On the _[!UICONTROL Admin]_ sidebar, go to **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   If it is your first time accessing Amazon sales channel or if your API key requires updating, the system prompts you through the process.

   ![Get and Add the Amazon API Key Prompt](assets/amazon-api-verification-prompt.png){width="500"}

1. Click **[!UICONTROL Sign in]** to access your [!DNL Commerce] web account.

    The Commerce accounts page opens in a new browser tab.

   - If you are logged into your [!DNL Commerce] account, the _[!UICONTROL API Portal]_ section of the _[!UICONTROL My Account]_ page appears automatically.

   - If you are not logged in, you are prompted to enter your [!DNL Commerce] account username and password before the _[!UICONTROL API Portal]_ tab appears.

   - If you do not have an account, visit [the [!DNL Commerce] account page](https://account.magento.com/customer/account/login/){target="_blank"} and register. This account should be part of your company or business.

1. If needed, you can view and generate API keys on the _[!UICONTROL API Portal]_ tab in your [!DNL Commerce] account.

   To create an API key, enter a description like `Amazon Sales Channel` and click **[!UICONTROL Add New]**. The new key is generated and shown with the name you entered. Click **[!UICONTROL Copy]** to copy the new key.

    ![Generate or copy an API key](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. With the new key generated and copied, return to the _[!UICONTROL Amazon Sales Channel]_ tab in the browser.

1. On the _[!UICONTROL Welcome to Amazon Sales Channel]_ page, click **[!UICONTROL Add the key]**.

   The browser exits Amazon sales channel and a store configuration page opens the _[!UICONTROL Api Keys]_ page in the [!DNL Commerce] Admin. You can open this page manually when you go to **[!UICONTROL Stores]** > _[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, expand **[!UICONTROL Services]** in the left panel, and choose **[!UICONTROL Magento Services]**.

1. Paste the copied key for **[!UICONTROL Production Api key]**.

1. Click **[!UICONTROL Save Config]**. You can now return to Amazon sales channel.

    ![Adding your API Key in your store configuration](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. On the _[!UICONTROL Admin]_ sidebar, go to **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Re-accessing Amazon sales channel triggers [!DNL Commerce] verify and validate your API key and allows you to continue.

   If you are prompted to verify the key again, repeat this _Add and Verify_ process.

![Next icon](assets/btn-next.png) [**Continue to Store Integration**](./store-integration.md)
