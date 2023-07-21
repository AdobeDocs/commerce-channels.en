---
title: 'Connect [!DNL Channel Manager] to [!DNL Walmart Marketplace]'
description: "Connect a Commerce store view to [!DNL Walmart Marketplace] to create the sales channel to manage Commerce product listings, inventory, price, and orders for Walmart Marketplace sales."
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
role: Admin, Developer
feature: Sales Channelss, Install, Integration
---
# Connect [!DNL Channel Manager] to [!DNL Walmart Marketplace]

After installing Channel Manager on your [!DNL Commerce] instance, create a sales channel in Channel Manager and configure the credentials to connect [!DNL Channel Manager] to [!DNL Walmart Marketplace].

1. [Create the sales channel](#create-the-sales-channel) by selecting the [!DNL Commerce] store for product listings.

1. [Connect the channel to [!DNL Walmart Marketplace] by adding [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Complete sales channel setup](#complete-sales-channel-store-setup) to manage listings, inventory, pricing, and orders for your [!DNL Walmart Marketplace] product assortment.

>[!NOTE]
>
>Channel Manager requires a one-to-one connection between a Walmart account and a [!DNL Commerce] store view. You cannot connect the same store view to multiple Walmart accounts.

## Create the sales channel

1. From the Admin, open [!DNL Channel Manager] by selecting **[!UICONTROL Marketing** > _Channels_ > **Channel Manager]**.

1. In the **[!UICONTROL Marketplaces available to connect]** section, select **[!UICONTROL Get Started]**.

   ![Connect new [!DNL Walmart] store to [!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

1. If needed, set up your [!DNL Walmart Marketplace Seller] account.

1. Configure the store and connection:

   - Select **[!UICONTROL Add Credentials]**. 

   - Select the [!DNL Commerce] store view that offers the products you want to sell on the marketplace.

     ![Configure connection between [!DNL Commerce] and [!DNL Walmart Marketplace] from [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}

   - Enter a unique **[!UICONTROL store name]**.

   - Select the **[!UICONTROL Adobe [!DNL Commerce] site]** for product listings and order processing.

   - To receive notifications related to [!DNL Channel Manager], add an **[!UICONTROL email address]**.

1. Connect the channel to [!DNL Walmart Marketplace].

   -  Add the credentials for the [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) from your [!DNL Walmart Marketplace Seller] account.

   - If you don't have the credentials, get them from the [!DNL Walmart Marketplace Developer Portal] by selecting **[!UICONTROL Get API credentials]**.

     On the Developer Portal, select your region (US and Canada) and then log in.

     ![[!DNL Walmart Marketplace] account login](assets/walmart-marketplace-login-page.png){width="600"}

   - On the API key form, copy and save the **[!UICONTROL Client ID]** and **[!UICONTROL Client Secret]** values for the [!UICONTROL Adobe Inc Production API key] to a secure location.

     ![[!DNL Walmart Marketplace API key] configuration page](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

     >[!NOTE]
     >
     >If the [!DNL Adobe Inc] key is not listed in the Developer Portal, select **[!UICONTROL Add New Key for a Solution Provider]** to configure permissions and generate the key. For configuration details, see [Generate a [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Return to [!DNL Channel Manager] to add the credentials to the **[!UICONTROL Walmart Connection]** information.

     When you add credentials, Adobe hides the client secret and stores the value in a secure vault.

1. Select **[!UICONTROL Save Store]** to apply the configuration and connect to the [!DNL Walmart marketplace].

1. After connecting successfully, [complete store setup](complete-sales-channel-store-setup.md) from the **[!UICONTROL Channel Manager]** store page.

![Setup first store](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### Troubleshoot connection issues

If the connection to [!DNL Walmart] fails, see the [Walmart Marketplace FAQ](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"} for troubleshooting tips.

- From the [!DNL Walmart Developer Portal], verify that you copied the correct credentials for the production API key for [!UICONTROL Adobe Inc.]

- Verify that the access configuration for the [!UICONTROL Walmart Adobe API key] has the correct permissions. See [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Confirm that the [!DNL Walmart API] service is available from the [Walmart API status page](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"}.
