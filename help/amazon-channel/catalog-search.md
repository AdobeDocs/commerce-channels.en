---
title: Catalog Search
description: To set the attribute matching that helps to map eligible Commerce catalog products with Amazon listings, update the Catalog Search settings.
redirect_from: /sales-channels/asc/ob-catalog-search.html
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
---
# Catalog Search

_Catalog Search_ settings are part of your store listing settings. Listing settings are accessed from the [store dashboard](./amazon-store-dashboard.md).

These settings enable you to set attribute matching that help to map eligible [!DNL Commerce] products with Amazon listings. When mapped, Amazon activates actions related to pricing, quantity, overrides, and order and product synchronization.

Defining these mapping values increases the potential for exact matches, minimizing the need to manually match product listings. Adding the attributes as part of your [Pre-Setup Tasks](./amazon-pre-setup-tasks.md), Amazon sales channel has a higher potential for automatically matching your products during onboarding and syncs product data between Amazon and [!DNL Commerce].

If you only create the Amazon ASIN attribute (without adding ASIN values per product), your [!DNL Commerce] products might not automatically match your Amazon listings. You can [manually assign](./creating-assigning-catalog-products.md) your products. However, manual matching does not create the data elements required to share and sync your product data.

>[!IMPORTANT]
>
>If you manually matched a product and you want to update an ASIN, UPC, or other data element for the product, you must update the data in two places. Update it in your [!DNL Commerce] catalog and in your Amazon listing in your [!DNL Amazon Seller Central] account.

It is a best practice to map these attributes and values if available. Completing this mapping is not required, but is beneficial for product matching and required for proper catalog syncing between Amazon and [!DNL Commerce].

If you want to add attributes, see [Create Product Attributes for Amazon Matching](./ob-creating-magento-attributes.md).

## Configure [!UICONTROL Catalog Search] settings

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the _[!UICONTROL Catalog Search]_ section.

1. For **[!UICONTROL ASIN]**, choose the product attribute you created for the Amazon ASIN value.

   An ASIN ([!DNL Amazon Standard Identification Number]) is a unique block of ten letters and/or numbers that identify items. For books, the ASIN is the same as the ISBN number, but for all other products a new ASIN is created when the item is uploaded to their catalog. You can find an items ASIN on the product detail page on Amazon, along with further details relating to the item.

1. For **[!UICONTROL EAN]**, choose the product attribute you created for the Amazon EAN value.

   The European Article Number (EAN) is a barcode standard, a 12 or 13-digit product identification code. Each EAN uniquely identifies the product, manufacturer, and its attributes; typically, the EAN is printed on a product label or packaging as a bar code. Amazon requires EAN codes to improve quality of search results and the quality of the catalog. You can obtain EANs from the manufacturer.

1. For **[!UICONTROL GCID]**, choose the product attribute you created for the Amazon GCIN value.

   The Global Catalog Identifier (GCID) is an ID for products that do not have a UPC code or ISBN. Amazon's Brand Registry allows you to register as a brand owner and create a unique ID for products.

1. For **[!UICONTROL ISBN]**, choose the product attribute you created for the Amazon ISBN value.

   The International Standard Book Number (ISBN) is a unique commercial book identifier barcode. Each ISBN code uniquely identifies a book. An ISBN has either ten or 13 digits. All ISBN assigned after Jan 1, 2007 have 13 digits.

1. For **[!UICONTROL UPC]**, choose the product attribute you created for the Amazon UPC value.

   The Universal Product Code (UPC) is a 12-digit bar code used extensively for retail packaging in United States.

1. For **[!UICONTROL General Search]**, choose the product attribute you want to use for a general search match.

   This attribute is one that you can select to match [!DNL Commerce] products to the appropriate Amazon listing. General search uses keyword searches from your catalog. As such, it is recommended to use a [!DNL Commerce] attribute that carries relevant keywords, such as the product SKU or product name. General search may return many possible matches, and in such cases, you can select the appropriate Amazon listing from the possible matches. A common selection for this field is `Product Name`.

1. When complete, click **[!UICONTROL Save listing settings]**.

![Catalog Search](assets/amazon-catalog-search.png){width="500" zoomable="yes"}

|Field|Description|
|--- |--- |
|[!UICONTROL ASIN]|A unique block of 10 letters and/or numbers that identify items.<br><br>ASIN stands for the [!DNL Amazon Standard Identification Number]. An ASIN is a unique block of 10 letters and/or numbers that identify items. For books, the ASIN is the same as the ISBN number, but for all other products a new ASIN is created when the item is uploaded to their catalog. You can find an items ASIN on the product detail page on Amazon, along with further details relating to the item. |
|[!UICONTROL EAN (European Article Number)]|A 12- or 13-digit product identification code. The European Article Number (EAN) is a barcode standard, a 12 or 13-digit product identification code. Each EAN uniquely identifies the product, manufacturer, and its attributes; typically, the EAN is printed on a product label or packaging as a bar code. Amazon requires EAN codes to improve quality of search results and the quality of the catalog. You can obtain EANs from the manufacturer. |
|[!UICONTROL GCID (Global Catalog Identifier)]|The Global Catalog Identifier (GCID) is an ID for products that do not have a UPC code or ISBN. Amazon's Brand Registry allows you to register as a brand owner and create a unique ID for products that may not have a UPC or ISBN. |
|[!UICONTROL ISBN (International Standard Book Number)]|A 10- or 13-digit unique commercial book identifier barcode. The International Standard Book Number (ISBN) is a unique commercial book identifier barcode. Each ISBN code uniquely identifies a book. An ISBN has either ten or 13 digits. All ISBN assigned after Jan 1, 2007 have 13 digits. |
|UPC (Universal Product Code)|A 12-digit bar code. The Universal Product Code (UPC) is a 12-digit bar code used extensively for retail packaging in United States. |
|[!UICONTROL General Search]|Select an attribute. This attribute is one that you can select to match [!DNL Commerce] products to the appropriate Amazon listing. General search uses keyword searches from your catalog. As such, it is recommended to use a [!DNL Commerce] attribute that carries relevant keywords, such as the product SKU or product name. General search may return many possible matches, and in such cases, you can select the appropriate Amazon listing from the possible matches. A common selection for this field is `Product Name`.|

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
