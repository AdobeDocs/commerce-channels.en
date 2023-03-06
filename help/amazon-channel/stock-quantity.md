---
title: Stock/Quantity
description: To control syncing of product quantity details from your Commerce store to your [!DNL Amazon Seller Central] account, update the Stock/Quantity settings.
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
---
# Stock/Quantity

*[!UICONTROL Stock/Quantity]* settings are part of your store listing settings. Listing settings are accessed from the [store dashboard](./amazon-store-dashboard.md).

These settings are used to sync the product quantity details from your [!DNL Commerce] storefront to the quantity on your [!DNL Amazon Seller Central] account. This tool is powerful and can be used for additional advertising by displaying urgency to the buyer while keeping your inventory organized. For example, some merchants may have 150 items of a particular SKU in stock in their warehouse and want to make sure that Amazon shoppers can purchase all of their inventory. Other merchants may wish to only list one item at a time to create a sense of scarcity to the end user. In this case, set the *[!UICONTROL Maximum Listed Quantity]* to `1`.

Quantity is a regional attribute and based on the **[!UICONTROL Amazon Marketplace Country]** setting define during [store integration](./store-integration.md). When a change is made to a product's quantity, the change affects all Amazon listings that share that [!DNL Amazon Seller SKU] in your Amazon stores that sell in the same country. A change to a shared [!DNL Amazon Seller SKU] in the United States does not affect your Amazon stores set up for a different country. Your first Amazon store that is integrated (with the oldest creation date) controls priority in the quantity settings.

>[!NOTE]
>
>For Adobe Commerce and Magento Open Source 2.3.x users, Amazon sales channel supports the use of the Inventory Management extension without any additional setup. See [Managing Inventory](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}.

## Configure stock/quantity settings {#configure-stock--quantity-settings}

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the **[!UICONTROL Stock / Quantity]** section.

1. For **[!UICONTROL Out-of-Stock Threshold]** (required), enter a numerical value for the lowest quantity of a product in order to keep the product eligible for its Amazon listing.

   The default is `0`. If your [!DNL Commerce] product stock goes lower than this number, the respective Amazon listing is ineligible for sales through Amazon.

1. For **[!UICONTROL Maximum Listed Quantity]** (required), enter a numerical value for the quantity you wish to show in your Amazon listing.

   This setting lists all your eligible Amazon listings at the entered value. When an item is sold, the Amazon listing quantity does not change. The listing quantity available always uses this value, even when your actual product quantity is higher or lower. This setting is typically used when you do not manage product inventory. For example, you may have a product with a quantity of 80 in your [!DNL Commerce] catalog. With set to `10`, the Amazon listing always displays a quantity available of `10` and does not change when sale is made for the product.

1. For **[!UICONTROL "Do Not Manage Stock" Quantity]** (required), enter a quantity value to show for your Amazon listings.

   Amazon requires that you publish an available quantity. For [!DNL Commerce] products that are set to not manage stock but you want to list them on Amazon, the listing is published with available quantity entered here.

1. When complete, click **[!UICONTROL Save listing settings]**.

![Stock/quantity settings](assets/amazon-stock-quantity.png)

|Field|Description|
|---|---|
|[!UICONTROL Out-of-Stock Threshold]|Enter a numerical value for the lowest quantity of a product in order to keep the product eligible for its Amazon listing (default is `0`).<br><br>If your [!DNL Commerce] product stock goes lower than this number, the respective Amazon listing is ineligible for sales through Amazon.|
|[!UICONTROL Maximum Listed Quantity]|Enter a numerical value for the quantity you want to show in your Amazon listing.<br><br>When an item is sold, the Amazon listing republishes with the quantity entered here. This setting is typically used when you do not manage product inventory.<br><br>For example, you enter the Maximum Listed Quantity value as `10`. Your actual quantity for a product is `80`. Because you have set this value at `10`, the Amazon listing always displays a quantity available of `10`. The quantity available is always displayed with the value defined, even when your stock quantity is lower.|
|[!UICONTROL "Do Not Manage Stock" Quantity]|Enter a value for your display quantity for your Amazon listings.<br><br>Amazon requires that you publish an available quantity. For [!DNL Commerce] products that are set to not manage stock but you want to list them on Amazon, the listing is published with available quantity of the value entered here.|

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## Example: Maximum listed quantity

When an item is sold, the Amazon listing relists it at this quantity.

For example, if you set *[!UICONTROL Maximum Listed Quantity]* as `12`, the Amazon listing shows a quantity of 12 even though the product has a [!DNL Commerce] quantity of 80:

![Maximum listed quantity example 1](assets/amazon-max-listed-quantity.png)

If you set your *[!UICONTROL Maximum Listed Quantity]* as `1`, all eligible products are listed with a quantity of `1`. When an item is sold, the system looks to your [!DNL Commerce] product and, if additional stock exists, relists the item on Amazon with a quantity of `1`.

This option might be valuable for products that are typically ordered at a quantity of 1. It also increases urgency for the shopper when viewing your Amazon listing.

![Maximum listed quantity example 2](assets/amazon-max-listed-quantity-1.png)
