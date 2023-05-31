---
title: Inventory and Price Updates
description: '[!DNL Channel Manager] syncs inventory and price updates between the [!DNL Commerce] store and [!DNL Walmart Marketplace] so that you can manage your sales channel operations from the [!DNL Commerce] Admin'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
---
# Update Inventory and Pricing

[!DNL Channel Manager] tracks inventory and pricing for products in the [!DNL Commerce] product catalog and synchronizes updates to the connected sales channel and [!DNL Walmart Marketplace]. The sync operation ensures that product listings reflect current stock quantity and pricing.


>[!IMPORTANT]
>
>After [!DNL Channel Manager] is installed and configured, all inventory, price, and order updates are synchronized automatically. If you already sell on Walmart Marketplace, make sure to disable any other integrations that update the product and order data. Then, verify that inventory stock levels and prices in the [!DNL Commerce] storefront are accurate and match the data in [!DNL Walmart Marketplace] before you connect [!DNL Channel Manager] to the live marketplace store.


## Inventory updates

When product inventory levels change in [!DNL Commerce], [!DNL Channel Manager] syncs updates to the [!DNL Walmart Marketplace]. It can take up to 10 minutes for inventory updates to sync across the sales channel to the [!DNL Walmart marketplace].

* **Updates to stock quantity in product catalog**—When [!DNL Commerce] stock quantity changes because of [manual stock quantity changes](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), refunds, or cancellations, [!DNL Channel Manager] syncs the change to connected channels and [!DNL Walmart Marketplace].

* **Reduce stock quantity to reflect [!DNL Walmart Marketplace] orders**—After a [!DNL Walmart Marketplace] order syncs to [!DNL Channel Manager], [!DNL Channel Manager] sends the update to the [!DNL Commerce] order system. [!DNL Commerce] adjusts stock quantities based on the order. Then, the updated quantity is synced to [!DNL Walmart Marketplace]. Until the sync operations are complete, you might see different quantities in the sales channel listings and [!DNL Walmart].

>[!IMPORTANT]
>
>After a [!DNL Walmart Marketplace] order syncs to [!DNL Channel Manager], inventory quantities and order information are updated only for refunds and cancellations initiated from [!DNL Commerce]. If an order is refunded or canceled from the [!DNL Walmart marketplace], process the change from [!DNL Commerce] to ensure the accuracy of [!DNL Commerce] inventory quantities and order information.

## Price updates

When the product price changes in [!DNL Commerce], [!DNL Channel Manager] syncs the update to the [!DNL Walmart Marketplace]. It can take up to five minutes for the price change to be displayed in the [!DNL Walmart Marketplace] listing.

### Manage pricing for a connected product

1. From the [!UICONTROL Admin], select **[!UICONTROL Catalog > Products]**.
1. In the product grid, find the product to update and select **[!UICONTROL Edit]**.
1. Review and update the price as needed.
1. **[!UICONTROL Save]** the change.

For help with managing product price configuration in [!DNL Commerce], see [Manage Pricing](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
