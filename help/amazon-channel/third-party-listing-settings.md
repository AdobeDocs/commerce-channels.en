---
title: Third-party Listings
description: Update the third-party listing settings determine if your Commerce catalog imports products from your existing Amazon Seller Central listings.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
---
# Third-party Listings

The third-party listing settings are part of your store listing settings. Listing settings are accessed from the [store dashboard](./amazon-store-dashboard.md).

These settings determine if your [!DNL Commerce] catalog imports products from your existing [!DNL Amazon Seller Central] listings. It is a best practice to import listings from Amazon, to ensure that all listings have matching [!DNL Commerce] products. When your listings are part of your [!DNL Commerce] catalog, you can manage all of your products from a single catalog and use Amazon sales channel features. These features include fulfillment and order management with Amazon, intelligent repricing, and quantity management.

When configured to import your Amazon listings, Amazon sales channel imports your Amazon listings into your [!DNL Commerce] catalog, attempting to match them to existing products. If a match is not automatically found, you can import the Amazon listing as a new [!DNL Commerce] product or manually match the listing to a product.

If you choose to import your Amazon listings, choose the [!DNL Commerce] attributes with values for Amazon Seller SKU and Amazon ASIN. If you do not have [!DNL Commerce] [product attributes](./ob-creating-magento-attributes.md), consider creating and assigning them. Mapping these attributes helps correctly match imported Amazon listings to your [!DNL Commerce] products.

The initial listing import initiates when [store integration](./store-integration.md) is complete. Afterward and based on your cron settings, [!DNL Commerce] continually checks for newly added Amazon listings (not created in Amazon Sales Channel) and updates your [!DNL Commerce] catalog according to your third-party listings settings.

## Configure third-party listing settings

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the _[!UICONTROL Third Party Listings]_ section.

1. For **[!UICONTROL Import Third Party Listings]** (required), choose an option:

    - `Import Listing` - (Default) Choose when you want product information from your Amazon listings to import into your [!DNL Commerce] product catalog. This option is the default and is recommended.

    - `Do Not Import Listing` - Choose when you want to manually [create and assign new products](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) to your [!DNL Commerce] catalog for your Amazon listings.

   >[!NOTE]
   >The following options fields are only active when set to `Import Listing`.

1. For **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, choose the [!DNL Commerce] attribute that matches to the Amazon Seller SKU value.

1. For **[!UICONTROL Attribute That Contains Amazon ASIN]**, choose the [!DNL Commerce] attribute that you created and match it to the Amazon ASIN.

   >[!NOTE]
   >If you did not create these [!DNL Commerce] attributes for your Amazon listings, see [Creating Attributes for Amazon Matching](./ob-creating-magento-attributes.md).

1. When complete, click **[!UICONTROL Save listing settings]**.

![Third party listings](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

|Field|Description|
|---|---|
|[!UICONTROL Import Third Party Listings]|Required. Options:<ul><li>**[!UICONTROL Import Listing]** - (Default) Choose when you want product information from your Amazon listings to import into your [!DNL Commerce] product catalog. </li><li>**[!UICONTROL Do Not Import Listing]** - Choose when you want to manually [create and assign new products](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) to your [!DNL Commerce] catalog for your Amazon listings.</li></ul>|
|[!UICONTROL Attribute That Contains Amazon Seller SKU]|Only active when set to `Import Listing`.<br>Choose the [!DNL Commerce] attribute as a match to the Amazon attribute for the Amazon Seller SKU. If this attribute does not exist, see [Creating Amazon Product Attributes for Amazon Matching](./ob-creating-magento-attributes.md). If needed, review your [!DNL Commerce] [attributes](./managing-attributes.md) and create or edit an attribute to match to this Amazon data.|
|[!UICONTROL Attribute That Contains Amazon ASIN]|Only active when set to `Import Listing`.<br>Choose the [!DNL Commerce] attribute that matches to the Amazon attribute for the Amazon ASIN. If this attribute does not exist, see [Creating Amazon Product Attributes for Amazon Matching](./ob-creating-magento-attributes.md). If needed, review your [!DNL Commerce] [attributes](./managing-attributes.md) and create or edit an attribute to match to this Amazon data.|

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
