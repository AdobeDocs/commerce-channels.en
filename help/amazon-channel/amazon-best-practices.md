---
title: Best Practices and Limitations for Amazon sales channel
description: Review the best practices and limitations when using the Amazon sales channel for Adobe Commerce and Magento Open Source.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
---
# Best Practices and Limitations for Amazon Sales Channel

Best practices include:

- Amazon sales channel can affect your Amazon listings by increasing or decreasing prices, synchronizing product information (including available stock), and adding, updating, and ending (deleting) listings. Review your listings by status during your setup and adjust your settings ([listing settings](./listing-settings.md), [listing rules](./listing-rules.md), [pricing rules](./pricing-products.md), [overrides](./overrides.md), and so on) before completing your store setup. These settings can also be modified after setup, as needed.

- Amazon sales channel can set your pricing rules to automatically adjust your listing price. Automated pricing safeguards include the [floor price](./floor-price.md) and [optional ceiling price](./optional-ceiling-price.md) features of [Intelligent repricing rules](./intelligent-repricing-rules.md). Use of these safeguards helps ensure that your listing prices do not go below your cost or above a defined price.

- Data syncing between Amazon sales channel and Amazon is controlled by your [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) settings. Built-in throttling between [!DNL Commerce] and Amazon helps to ensure smooth and efficient data transmission, but during high eCommerce traffic times (such as Black Friday), Amazon's systems could take longer than usual to update. Set your [!DNL Commerce] cron to run once every five minutes.

- Amazon sales channel imports your Amazon order information. To manage your Amazon orders in Amazon sales channel, you must ensure that your [order settings](./order-settings.md) are defined to import and create a corresponding [!DNL Commerce] order for each Amazon order. If it is not defined, you can only view your Amazon order information. All taxes for sales through Amazon are still managed and remitted via your [!DNL Amazon Seller Central] account. In some states, Amazon is required to automatically collect and remit taxes. For other states, sellers have the option of calculating taxes manually or automatically. See [Amazon: Tax Policies](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&language=en_US/){target="_blank"}. You might be required to log into your [!DNL Amazon Seller Central] account to view Amazon tax policy documentation.

- For UK regions, it is best  practice to enroll in the [Amazon VAT Calculation Service](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"} before onboarding Amazon sales channel.

   
   >[!NOTE]
   >
   >It may take 10-14 days for Amazon to verify and activate your VAT Calculation Service account.

Limitations include:

- Bundle, gift card, and grouped product types that are part of your [!DNL Commerce] catalog are not supported by Amazon sales channel for listing to Amazon.

- Amazon sales channel cannot create a listing for a product that does not have an existing or previous Amazon listing. If a product does not exist in [!DNL Amazon Seller Central] with an ASIN, it must be added in [!DNL Amazon Seller Central] so that Amazon can assign the product an ASIN. After a product is added in Amazon and a listing is created, the listing can be matched to your catalog in Amazon sales channel and synced.
