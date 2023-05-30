---
title: Store integration with an [!DNL Amazon Seller Account]
description: Before you start the onboarding process, you must create (add) an Amazon Sales Channel store and connect it to your Amazon Seller Account.
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
---
# Store integration with an [!DNL Amazon Seller Account]

To get started with Amazon sales channel, you must create (add) an Amazon sales channel store and connect it to your [!DNL Amazon Seller Account]. These two steps integrate your [!DNL Commerce] and Amazon accounts to share data, sync products, and more.

_You need the primary log-in credentials for your [!DNL Amazon Seller Central] account (the email or phone used to create the seller account) to connect your store._

>[!NOTE]
>
>After your first store integration, you will be prompted annually to renew your Amazon sales channel connection to Amazon by granting access again. You can renew or revoke this authorization in the _Current Authorizations_ table in the _Amazon MWS Developer Permissions_ section of the **Settings** > **User Permissions** page of your Seller Central account.

## Add an Amazon store

1. On the _Admin_ sidebar, go to **Marketing** > _Channels_ > **Amazon Sales Channel**.

    When adding your first Amazon sales channel store, the _Pre-Setup Tasks_ modal appears. After your first store is added, pre-setup tasks can be accessed on the [Amazon sales channel home](./amazon-sales-channel-home.md) page under _Learning and Preparation_ in the left-side menu.

1. Click **[!UICONTROL Add Amazon Store]**.

    The _[!UICONTROL Add Amazon sales channel]_ page opens.

    ![Add the Amazon sales channel store](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. For **[!UICONTROL Magento Website to use for Amazon Listing]**, choose which of your [!DNL Commerce] websites to connect for this Amazon sales channel store.

    This setting also defines the default [!DNL Commerce] store for [importing Amazon orders](./order-settings.md).

1. For **[!UICONTROL Email Address]**, enter your preferred contact email address.

1. For **[!UICONTROL New Store Name]**, enter a descriptive name for your new Amazon sales channel store.

   >[!NOTE]
   >
   >This name is used as a [!DNL Commerce] reference only and identifies the store on the [Amazon sales channel home](./amazon-sales-channel-home.md) page. You want to make it something your team can easily identify. For example, your Amazon store that sells in the United States region might be named `Amazon Store USA`.

1. For **[!UICONTROL Amazon Marketplace Country]**, choose the region/country in which this Amazon sales channel store sells products. Options:

    - United States
    - Canada
    - Mexico
    - United Kingdom

1. In the _[!UICONTROL Map your Magento attributes to Amazon]_ section, do the following:

    - For **[!UICONTROL Product ID on the Amazon market]**, choose the Amazon attribute to map to the [!DNL Commerce] attribute selected below.

      This ID helps to correctly match corresponding products in your [!DNL Commerce] catalog.

    - For **[!UICONTROL Map a Magento attribute]**, choose the [!DNL Commerce] product attribute to map to the Amazon attribute selected above.

      [Mapping attributes](./ob-creating-magento-attributes.md) helps ensure that your Amazon listing correctly matches to the corresponding product in your [!DNL Commerce] catalog.

1. Click **[!UICONTROL Connect]**.

   The dialog closes and the new store appears on the [Amazon sales channel home](./amazon-sales-channel-home.md) page with a confirmation message.

## Connect a store to [!DNL Amazon Seller Central]

1. On the store dashboard, click **[!UICONTROL Connect store]** on the store card to launch [!DNL Amazon Seller Central] in a new tab.

1. Enter your [!DNL Amazon Seller Central] account credentials and click **[!UICONTROL Sign in]**.

   To complete this connection, you must sign in to your [!DNL Amazon Seller Central] account using the login credentials for the primary user (the email or phone used to create the seller account).

1. If prompted, complete the Amazon Two-Factor Authorization (2FA) by entering the code you receive from Amazon and click **[!UICONTROL Sign in]**.

1. On the _[!UICONTROL Amazon Marketplace Web Service]_ confirmation page, select the "[!UICONTROL I understand...]" checkbox and click **[!UICONTROL Next]**.

1. On the _[!UICONTROL You are almost done]_ message, click **[!UICONTROL Continue]**.

   You have granted Amazon sales channel permission to access and share data with your [!DNL Amazon Seller Central] account. The Amazon page closes and a confirmation message appears.

   The [Amazon sales channel home](./amazon-sales-channel-home.md) page opens showing your Amazon store cards.

   To view the store dashboard, click **[!UICONTROL View Store]** on the store card.

![Amazon sales channel home with new store card](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

Your new Amazon sales channel store is now connected to your [!DNL Amazon Seller Central] account.

![Next icon](assets/btn-next.png) [**Continue to Create a Listing Rule**](./ob-create-listing-rule.md)
