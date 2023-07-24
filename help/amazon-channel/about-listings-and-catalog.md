---
title: Amazon and the Commerce catalog
description: The Amazon sales channel imports your Amazon listings into your Commerce backend, and continually syncs with products and sales.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalog
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
---
# Amazon and the [!DNL Commerce] Catalog

Your Adobe Commerce or Magento Open Source backend includes a catalog with all products and associated settings and information (images, options, prices, and more) and order and shipping configurations. Your [!DNL Amazon Seller Central] account also has a catalog and order configurations, tracking strictly your sales through the [!DNL Amazon Marketplace].

To better manage and review your product catalog and sales through one location, Amazon sales channel imports your Amazon listings into your [!DNL Commerce] backend, continually syncs with products and sales, and reports issues and trends. It supports integrations with multiple [!DNL Amazon Seller Central] accounts, tracking all data through the single interface for multiple storefronts.

## Product attributes

Adobe Commerce and Magento Open Source manage catalog syncs with the use of product [attributes](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) to define product settings and data. Amazon also uses attributes, to be mapped through onboarding. During [pre-setup tasks](./amazon-pre-setup-tasks.md) for Amazon sales channel, you define additional Amazon attributes (if needed) to ensure correct product mappings when importing your Amazon listings into your [!DNL Commerce] catalog. These attributes include UPC, EAN, ISBN, and ASIN ([!DNL Amazon Standard Identification Number]). Through onboarding, products sync between Amazon and [!DNL Commerce] catalogs using your attributes. Proper mapping of your [!DNL Commerce] and Amazon products ensures a continual synchronization of product information, orders, and inventory.

If you do not have these attributes created or configured for your catalog, you should add a [!DNL Commerce] [product attribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) and values to your products before onboarding. When an Amazon attribute is imported, it can be used for search, navigation, price rules, and much more. See [What Do ASIN, UPC, EAN, ISBN, SKU and Other Barcodes Mean?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

After onboarding, you can manage and update your product attributes and Amazon mappings at any time.

## Product listings

An Amazon listing is a product page for every product you sell through the [!DNL Amazon Marketplace], displaying product descriptions, prices, images, and more mapped through attributes. During onboarding, you can configure your [!DNL Commerce] products can be automatically published to Amazon listings. You can also import your existing Amazon listings by mapping them to your [!DNL Commerce] products.

When you have created a listing [!DNL Commerce] products, they are submitted to Amazon for approval. Most successful listings are approved within a few hours. If your listing is approved, it appears in the [!DNL Amazon Marketplace] for immediate orders by customers. The [!DNL Amazon Sales Channel] extension provides a set of tabs to review Amazon listings. Depending on the issue or required data, you should review your [!DNL Amazon Seller Central] account for specific details on these listings.

- [Active](./active-listings.md): Lists approved product listings available through the marketplace.

- [Ready to List](./ready-to-list.md): Lists products meeting listing rules requirements and ready to publish to Amazon.

- [Inactive](./inactive-listings.md): Lists products that are not available on the marketplace due to being blocked for a specific reason (such as branding issue), closed and requiring relisting, and so on.

- [Ineligible](./ineligible-listings.md): Due to the listing rules, lists product that cannot be actively listed on the marketplace (such as `0` quantity or sell dates).

- [Incomplete](./incomplete-listings.md): Lists products missing required information. Update the product data for another review.

- [Ended](./ended-listings.md): Lists product listings eligible for listing but manually removed from Amazon. You can relist these products.

## Syncing data

Adobe Commerce and Magento Open Source communicate product and order data between your [!DNL Amazon Seller Central] account and the [!DNL Commerce] backend. The continual updates provide a single source through [!DNL Commerce] to manage and maintain your inventories, fulfilling orders, tracking sales, and reducing overhead and duplication of work. Reporting captures the latest data for tracking trends and resolving communication issues caught between the two systems.

All syncing is managed by a [cron job](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html), set to update every five minutes in your [Pre-Setup Tasks](./amazon-pre-setup-tasks.md).
