---
title: About Amazon and the Commerce Catalog
---

# About Amazon and the [!DNL Commerce] catalog

Your Adobe Commerce or Magento Open Source backend includes a catalog with all products and associated settings and information (images, options, prices, and more) and order and shipping configurations. Your [!DNL Amazon Seller Central] account also has a catalog and order configurations, tracking strictly your sales through the [!DNL Amazon Marketplace].

To better manage and review your product catalog and sales through one location, [!DNL Amazon Sales Channel] imports your Amazon listings into your [!DNL Commerce] backend, continually syncs with products and sales, and reports issues and trends. It supports integrations with multiple [!DNL Amazon Seller Central] accounts, tracking all data through the single interface for multiple storefronts.

## Product attributes

Adobe Commerce and Magento Open Source manage catalog syncs with the use of product [attributes](https://docs.magento.com/user-guide/catalog/product-attributes.html) to define product settings and data. Amazon also uses attributes, to be mapped through onboarding. During [pre-setup tasks](./amazon-pre-setup-tasks.md) for [!DNL Amazon Sales Channel], you will define additional Amazon attributes if needed to ensure correct product mappings when importing your Amazon listings into your [!DNL Commerce] catalog. These attributes include UPC, EAN, ISBN, and ASIN ([!DNL Amazon Standard Identification Number]). Through onboarding, products sync between Amazon and [!DNL Commerce] catalogs using your attributes, especially these. Proper mapping of your [!DNL Commerce] and Amazon products ensures a continual synchronization of product information, orders, and inventory.

If you do not have these attributes created or configured for your catalog, we recommend adding a [!DNL Commerce] [product attribute](https://docs.magento.com/user-guide/catalog/product-attributes.html) and values to your products prior to onboarding. When an Amazon attribute is imported, it can be used for search, navigation, price rules, and much more. For more information on these attributes, see [Amazon: What are UPCs, EANs, ISBNs. and ASINs?][1]

After onboarding, you can manage and update your product attributes and Amazon mappings at any time.

## Product listings

An Amazon listing is a product page for every product you sell through the [!DNL Amazon Marketplace], displaying product descriptions, prices, images, and more mapped through attributes. During onboarding, you can configure your [!DNL Commerce] products can be automatically published to Amazon listings. You can also import your existing Amazon listings by mapping them to your [!DNL Commerce] products.

When you have created a listing [!DNL Commerce] products, they are submitted to Amazon for approval. Most successful listings are approved within a few hours. If your listing is approved, it will display in the [!DNL Amazon Marketplace] for immediate orders by customers. The [!DNL Amazon Sales Channel] provides a set of tabs to review Amazon listings. Depending on the issue or required data, you may need to review your [!DNL Amazon Seller Central] account for specific details on these listings.

- [Active](./active-listings.md): Lists approved product listings available through the marketplace.

- [Ready to List](./ready-to-list.md): Lists products meeting listing rules requirements and ready to publish to Amazon.

- [Inactive](./inactive-listings.md): Lists products not available on the marketplace due to being blocked for a specific reason (such as branding issue), closed and requiring relisting, etc.

- [Ineligible](./ineligible-listings.md): Due to the listing rules, lists product that cannot be actively listed on the marketplace (such as `0` quantity, sell dates, etc).

- [Incomplete](./incomplete-listings.md): Lists products missing required information. Update the product data for another review.

- [Ended](./ended-listings.md): Lists product listings eligible for listing but manually removed from Amazon. You can relist these products.

## Syncing data

Adobe Commerce and Magento Open Source communicate product and order data between your [!DNL Amazon Seller Central] account and the [!DNL Commerce] backend. The continual updates provide a single source through [!DNL Commerce] to manage and maintain your inventories, fulfilling orders, tracking sales, and reducing overhead and duplication of work. Reporting captures the latest data for tracking trends and resolving communication issues caught between the two systems.

All syncing is managed by a [cron job](https://docs.magento.com/user-guide/system/cron.html), set to update every five minutes in your [Pre-Setup Tasks](./amazon-pre-setup-tasks.md).

[1]: https://www.amazon.com/gp/seller/asin-upc-isbn-info.html