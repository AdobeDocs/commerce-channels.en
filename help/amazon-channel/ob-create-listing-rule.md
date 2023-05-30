---
title: 'Onboarding: Create listing Rule'
description: While completing the Amazon sales channel onboarding process, create the initial listing rules for generating Amazon listings for your [!DNL Commerce] products.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
---
# Onboarding: Create listing Rule

Listing rules can be defined during onboarding, but can also be modified at any time. After onboarding, you can access the [listing rules](./listing-rules.md) on the store [dashboard](./amazon-store-dashboard.md).

## Create a listing rule during onboarding

1. After your store is connected, click **[!UICONTROL View Store]** for the added store.

   The store [dashboard](./amazon-store-dashboard.md) appears with the `No products listed to Amazon` message.

1. Click **[!UICONTROL Preview and List Eligible Products]**.

   The _[!UICONTROL Listing Rules]_ page appears.

1. Define your desired conditions for the eligibility of products to be listed on Amazon and click **[!UICONTROL Preview changes]**, or click **[!UICONTROL Preview changes]** to skip this step.

   See [Example: Define a Condition](./ob-define-condition-example.md).

1. Review your listings in the Listing Preview:

   ![Listing preview](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - Products listed on this tab are not eligible for Amazon listing based on your current listing rule settings.

      Ineligible products are not published to Amazon. If an ineligible product is already listed on Amazon and you match the Amazon listing to your [!DNL Commerce] catalog product, the quantity for the Amazon listing changes to `0` to prevent sales of the product. To manually remove a listing from Amazon, see [Ending an Amazon Listing](./end-listings-manually.md). Products that are not eligible by Amazon requirements are not listed here. Those products are listed on the [[!UICONTROL Inactive Listings] tab](./inactive-listings.md).

      To change an `Ineligible` listing to an `Eligible` listing, repeat this process and modify your listing rules.

   - **[!UICONTROL Eligible Listings]** - Products listed on this tab are eligible for Amazon listing based on your current listing rule setup and are eligible by Amazon requirements. This tab includes your existing Amazon listings that are imported (if you have **[!UICONTROL Import Third Party Listings]** set to `Import Listing` in your [Listing Settings](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - Products listed on this tab include your [!DNL Commerce] catalog products that are newly eligible for Amazon listing based on your current listing rule setup and create Amazon listings.

1. When complete, click **[!UICONTROL Save and Close]**.

   The store [dashboard](./amazon-store-dashboard.md) opens.

After onboarding a store is complete, the information sync between [!DNL Commerce] and Amazon is initiated. Your Amazon listings are imported into [!DNL Commerce] and attempt to match with products in your [!DNL Commerce] Catalog.

You can view your Amazon order information in the _[!UICONTROL Recent Orders]_ section of the store dashboard. See [Store Dashboard](./amazon-store-dashboard.md) or [Manage Orders](./managing-orders.md).

>[!IMPORTANT]
>
>There are some important store settings (listings, pricing, rules, fulfillment, more) that have default values for a new store. To ensure that your store is set up for your specific needs, review your [store settings](./default-store-settings.md) .

![Next icon](assets/btn-next.png) [**Continue to Default Store Settings**](./default-store-settings.md)
