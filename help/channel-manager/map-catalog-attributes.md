---
title: Map Catalog Attributes
description: 'Map attributes for matching [DNL! Commerce] products to existing [!DNL Walmart Marketplace] listings and synchronizing data between [!DNL Channel Manager] and [!DNL Walmart].'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
---
# Map Catalog Attributes

Before you connect listings from [!DNL Commerce] to [!DNL Walmart Marketplace], you must map at least one unique identifier from your [!DNL Commerce] catalog to the corresponding identifier from Walmart.

This step is required to match [!DNL Commerce] products to existing [!DNL Walmart] listings and to synchronize product data between [!DNL Commerce] and [!DNL Walmart]. The [!DNL Commerce] product must have at least one product attribute that matches one of the following Product Identifiers (Product IDs) required by [!DNL Walmart].

**Required [!DNL Walmart] product IDs**

| **Accepted Type** | **Name**                             | **Purpose**                                                                                                                                      | **Acceptable Digits** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN              | Global Trade Item                    | General purpose, used worldwide                                                                                                                  | 14 digits             |
| ISBN              | International Standard Book Number   | Paperback, Hardcover and Electronic Books                                                                                                        | 10 or 13 digits       |
| ISSN              | International Standard Serial Number | 8-digit serial number used to identify magazines, journals, newspapers, and periodicals of all kinds delivered on all media–print and electronic | 8 digits              |
| UPC               | Universal Product Code               | Standard retail tracking code                                                                                                                    | 12 digits             |

If your catalog does not have a matching attribute, [add or convert an existing catalog attribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

## Map unique identifiers

1. From the **[!UICONTROL Listings]** or **[!UICONTROL Orders]** page for the sales channel store, select **[!UICONTROL Channel Settings]**.

1. On **[!UICONTROL Channel Settings]**, select **[!UICONTROL Map Attributes]**.

   - Find the [!DNL Walmart Marketplace] attribute to map.

   - Select the corresponding attribute from the [!DNL Commerce] store catalog.

     The following example maps the [!UICONTROL Walmart Marketplace UPC] attribute to the UPC attribute in the product catalog.

     ![Map attributes for product match criteria](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - Select **[!UICONTROL Save]**.
