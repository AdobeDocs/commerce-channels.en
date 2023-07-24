---
title: Default store settings for Amazon listings
description: Modify the default Commerce settings to customize the Amazon Sales Channel for your store.
role: Admin
feature: Sales Channel, Integration, Configuration
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
---
# Default store settings for Amazon listings

After your store is connected and you've set up your first listing rule, the sync of data between Amazon and [!DNL Commerce] starts. There are several types of store settings that allow you to customize your store for your needs. Store settings are accessed on the store [dashboard](./amazon-store-dashboard.md).

Store settings include:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Control how your product catalog interacts with the [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Control how Amazon orders are managed.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Define which catalog products are eligible to be listed on Amazon.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Define how the Amazon list price is altered for qualified listings.

- **[!UICONTROL Store reports]** - [Competitive price analysis](./competitive-price-analysis.md) and [listing improvements](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Listing changes](./listing-changes-log.md) and [communication errors](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Review email and Amazon sales channel store name settings in the [!DNL Commerce] Admin.

## Some important default settings

| Setting                                | Default                                | Description                                                                                                                                                                                                                                                                                                                                                                                                          | Location                                                    |
|----------------------------------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders]      | `Enabled`                              | Creates corresponding [!DNL Commerce] orders when new orders are received from Amazon, allowing orders to be managed in the [[!DNL Commerce] Orders](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) workflow. When `Disabled`, Amazon orders import order information for review, but orders must be managed in your [!DNL Amazon Seller Central] account. | [Order Settings](./order-settings.md)                       |
| [!UICONTROL Customer Creation]         | `No Customer Creation (guest)`         | Customer data from Amazon orders is not imported into your [!DNL Commerce] database. Imported Amazon orders are processed as a guest checkout. If you want to build your [!DNL Commerce] customer database, you should change this setting to `Build New Customer Account`.                                                                                                                                          | [Order Settings](./order-settings.md)                       |
| [!UICONTROL Automatic List Action]     | `Automatically List Eligible Products` | [!DNL Commerce] catalog products (that meet Amazon's eligibility requirements) to automatically publish to Amazon and create Amazon Listings. If you want to manually review and publish your products, you should change this setting to `Do Not Automatically List Eligible Products`. Products waiting for manual publish appear on the [_Ready to List_](./ready-to-list.md) tab.                                | [Product Listing Actions](./product-listing-actions.md)     |
| [!UICONTROL Magento Price Source]      | `Price`                                | Defines the price source attribute used as the base for your Amazon listings. If you do not want to use the [!DNL Commerce] `Price` attribute as your base price to which your pricing rules are based, you should change this setting to a different attribute.                                                                                                                                                     | [Listing Price](./listing-price.md)                         |
| [!UICONTROL Product Fulfilled By]      | `Fulfilled by Merchant`                | The merchant fulfills all orders. If you use Fulfillment by Amazon or use a mix of fulfillment methods, you should change this setting.                                                                                                                                                                                                                                                                              | [Fulfilled by](./listing-price.md)                          |
| [!UICONTROL Listing Product Condition] | `New`                                  | If all your products are the same condition, you can select one of the Amazon condition options to represent all of your products. If your catalog contains products in different conditions (such as New, Used, and Refurbished), you must change this setting to `Assign Condition Using Product Attribute` and map your [!DNL Commerce] condition attributes to your Amazon listing conditions.                   | [Product Listing Condition](./product-listing-condition.md) |
| [!UICONTROL Listing Rules]             | none                                   | Define the rules used to determine which products Amazon sales channel publishes to Amazon. These rules provide many options to create simple to complex rules to include or exclude products as listings.                                                                                                                                                                                                           | [Listing Rules](./listing-rules.md)                         |
| Pricing Rules                          | none                                   | Define your Amazon listing price attribute different than the defined _[!UICONTROL Magento Price Source]_ in your [Listing Price](./listing-price.md). To adjust your listing price (up or down) against your _[!UICONTROL Magento Price Source]_ setting, create rules.                                                                                                                                             | [Pricing Rules](./pricing-products.md)                      |

For more information, see [Store Settings](./ob-store-review.md).
