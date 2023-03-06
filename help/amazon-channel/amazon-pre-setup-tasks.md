---
title: Pre-Setup Tasks
description: Review the required tasks to be completed before integrating your Adobe Commerce or Magento Open Source store in Amazon Sales Channel.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
---
# Pre-Setup Tasks

Before [Store Integration](./store-integration.md), you must ensure that your [!DNL Amazon Seller Central] account and your [!DNL Commerce] account are ready for the integration. To successfully integrate, there are some required pre-setup tasks.

When you set up your first Amazon store in Amazon sales channel, a list of setup tasks appears. It is recommended that you review these tasks before you [add an Amazon store](./store-integration.md). After adding your first store, you can review these tasks in the Learning and Preparation view of the Amazon sales channel [home page](./amazon-sales-channel-home.md).

## 1. Enable background tasks in [!DNL Commerce]

All products and data synced between [!DNL Commerce] and Amazon is managed by a [cron job](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}. When you complete tasks such as add or update listings and receive orders, a cron job sends and receives data between your [!DNL Commerce] backend and your [!DNL Amazon Seller Central] account.

- [Enable [!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}.

- For maximum performance, [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target="_blank"} to run once every five minutes.

## 2. Create your [!DNL Amazon Seller Central] account

Before you begin to set up your Amazon sales channel, you must have an active [!DNL Amazon Seller Central] account. If you don't have an existing Amazon Seller account in the [North America (US, CA, MX)](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} region, you can complete Amazon's seller account setup process.

Amazon sales channel requires a [!DNL Professional Seller] account on [!DNL Amazon Seller Central]. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. Make sure you are an approved Amazon seller

To integrate, you must have an approved [!DNL Amazon Seller Central] account. Your account must not have any restrictions for products or categories. Some products and categories require approval before creating listings. Review Amazon policies for category and product approval to ensure that your products are approved. See [Amazon: Categories and products requiring approval](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (Seller Central login required).

It is also important to ensure that you have configured the following in your [!DNL Amazon Seller Central] account:

- Ensure that your return policy is as good as or better than the Amazon return policy. See [Amazon: Return Policy](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- Ensure that your tax settings are configured. See [Amazon: Tax Policies](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (Seller Central login required).

- Ensure that your shipping methods are configured accurately. To set up the shipping methods that [!DNL Commerce] are offered to customers to fulfill your Amazon orders, update the [Amazon: Shipping Settings](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} in your [!DNL Amazon Seller Central] account.

## 4. Make sure that your VAT is configured for your stores

(Primarily used by UK sellers.) Amazon recommends signing up for the [Amazon VAT Calculation Service](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. If you choose a different method, you are responsible for VAT compliance.

>[!NOTE]
>
>It may take 10-14 days for Amazon to verify and activate your VAT Calculation Service account.

## 5. Increase the number of automatic catalog matches

During onboarding, Amazon sales channel uses product attributes to match your existing Amazon listings (if applicable) to existing products in your [!DNL Commerce] catalog. After onboarding, these product attributes are used to publish your [!DNL Commerce] catalog items to an Amazon listing and to sync your product data between [!DNL Commerce] and Amazon.

To have the highest number of [!DNL Commerce] products automatically match with Amazon listings, you should create a set of product attributes for your [!DNL Commerce] catalog. Before you set up your Amazon sales channel store, you should add [!DNL Commerce] product attributes to match these Amazon attributes, for example: ASIN, EAN, ISBN, UPC, or GCID. See [Create a product attribute in [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. Configure your currency and conversion (as needed)

If your Amazon store uses a different currency than is configured for your [!DNL Commerce] store, [enable the currency](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target="_blank"} and set the [currency conversion rate](https://docs.magento.com/user-guide/stores/currency-update.html){target="_blank"}.

## 7. Create a product condition attribute (as needed)

If your Amazon listings contain more than one product condition (such as _new_, _used_, or _like new_), create a [!DNL Commerce] attribute and assign condition values. You must map this attribute during onboarding to the Amazon Condition product attribute. See [Creating Attributes for Amazon](./ob-creating-magento-attributes.md).

## 8. Configure your [!DNL Amazon Seller Central] shipping method

To set up shipping methods that you want to offer for fulfilling your Amazon orders, refer to [Settings & Shipping Settings][10] in your [!DNL Amazon Seller Central] account.

## Additional configurations

When your Amazon account is set up and active, there are several [!DNL Commerce] recommendations that help streamline the Amazon sales channel onboarding process.

### Review and note any products that you want to exclude

You may not want some products to be listed on Amazon. Amazon sales channel has a listing rule engine that is used to determine which products are eligible for publishing to Amazon. [Listing rules](./listing-rules.md) allow you to select subsets of products to be published (or not published) to your [!DNL Amazon Seller Central] account, such as by category selection or by defining one or more product attributes. Like [!DNL Commerce] [catalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"} or [shopping cart](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target="_blank"} price rules, product attributes used for Amazon listing eligibility must have **[!UICONTROL Use for Promo Rule Conditions]** set to `Yes`. See the **[!UICONTROL Use for Promo Rule Conditions]** in [Product Attributes](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"}.

### Set your [!DNL Amazon Seller Central] region to inactive

To help facilitate error-free data transition during integration, it is recommended that you set your Amazon region to `Inactive` status in Settings > Account Info > Vacation Settings. Refer to [Amazon: Listing Status for Vacations][11]. When your setup is complete, change the status back to `Active` in Amazon.

![Next icon](assets/btn-next.png) [**Continue to Creating [!DNL Commerce] Attributes**](./ob-creating-magento-attributes.md)
