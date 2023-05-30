---
title: Product Listing Actions
description: Use the Product Listing Actions settings to define how your Commerce catalog interacts with Amazon.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
---
# Product Listing Actions

The Product listing actions settings are part of your store listing settings. Listing settings are accessed from the [store dashboard](./amazon-store-dashboard.md).

These settings define how your catalog interacts with Amazon. These settings:

- Indicate if your [!DNL Commerce] catalog products that meet Amazon eligibility requirements are automatically sent to your [!DNL Amazon Seller Central] account to create listings.

- Set the default handling time for an order. This value defines the number of days required for you to process and ship an order. For example, if someone selects 2-day shipping, that shipping transit time does not start until processing completes and packages are handed off to a carrier. The total delivery time is (handling time + transit time + any holidays).

## Configure settings

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the _[!UICONTROL Product Listing Actions]_ section.

1. For **[!UICONTROL Automatic List Action]** (required), choose an option:

   - `Automatically List Eligible Products` - (Default) Choose when you want your [!DNL Commerce] catalog products (that meet Amazon's eligibility requirements) to automatically publish to Amazon and create Amazon Listings.

   - `Do Not Automatically List Eligible Products` - Choose when you want to manually select your eligible [!DNL Commerce] catalog products and create Amazon listings. When chosen, catalog products that meet your listing criteria and contain all required information display on the [_[!UICONTROL Ready to List]_](./ready-to-list.md) tab for manual publish to Amazon.

1. For **[!UICONTROL Default Handling Time]** (required), enter the number of days needed for lead time before shipment.

   The default value is `2` days.

   >[!NOTE]
   >
   >This default handing time value is only effective for Amazon listings created through Amazon sales channel. Any Amazon listings that were created in your [!DNL Amazon Seller Central] account use the default handling time set in Amazon.

1. When complete, click **[!UICONTROL Save listing settings]**.

![Product listing actions](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

|Field|Description|
|--- |--- |
|[!UICONTROL Automatic List Action]|Options:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Recommended) Choose when you want your [!DNL Commerce] catalog products (that meet Amazon's eligibility requirements) to automatically publish to Amazon and create Amazon Listings. When chosen, the [_[!UICONTROL Ready to List]_](./ready-to-list.md) tab is not displayed. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Choose when you want to manually select eligible [!DNL Commerce] catalog products and create Amazon Listings. When chosen, catalog products that meet your listing criteria and contain all required information display on the [_[!UICONTROL Ready to List]_](./ready-to-list.md) tab for manual publishing.</li></ul>|
|[!UICONTROL Default Handling Time]|The numerical value that represents the number of days, in general, that it takes you to process and ship your orders. The default value is `2`. This value is used for Amazon listings created in [!DNL Commerce] and published to Amazon. The default handling time for Amazon listings before integrating with [!DNL Commerce] are not affected by this setting.<br><br>The value defined in Amazon sales channel does not replace the default handling time defined in an existing Amazon listing. When a **[!UICONTROL Handling Time Override]** is enabled and then removed, the Handling Time for an order reverts to the value defined here.<br><br>If you have products that have different handling times, you can create a Handling Time Override at the product-specific level. You can manage handling time overrides in the [_[!UICONTROL Overrides]_](./overrides.md) tab, giving you flexibility to manage your product fulfillment. If there is no handling time override in [!DNL Commerce] for a product, the handling time default is the value defined in the Amazon listing.<br><br>Handling Time is a regional attribute. When the value is changed for a listing, the change affects all listings that share the [!DNL Amazon Seller SKU] in all Amazon stores that exist for the same region (defined at [store integration](./store-integration.md)). However, changing the value for a shared [!DNL Amazon Seller SKU] in the North America region does not affect the same products listed in a store with a different defined region. The store for the region with the oldest creation date controls the priority for the Default Handling Time settings.|

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
