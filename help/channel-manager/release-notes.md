---
title: '[!DNL Channel Manager] Release Notes'
description: The latest release information for [!DNL Channel Manager] from Adobe Commerce.
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
---
# [!DNL Channel Manager] Release Notes

These release notes describe the initial release of [!DNL Channel Manager] and include:

![New](../assets/new.svg) New features
![Fixed issue](../assets/fix.svg) Fixes and improvements
![Known issue](../assets/bug.svg) Known issues


## v1.1.0

![New](../assets/new.svg)<!--CHAN-5204--> **Returns and Refunds**—You can now process Walmart Marketplace returns and refunds process for orders shipped through an Adobe Commerce and Magento Open Source Channel Manger store. Information and updates about returns and refunds are synchronized between Walmart and Adobe Commerce so that the current data is available in both the [!DNL Commerce] storefront and [!DNL Walmart Marketplace]. See [Return and refund orders](return-refund-orders.md).

![Fixed](../assets/fix.svg)<!--CHAN-5661--> Fixed the `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` error that occurred when resynchronizing Channel Manager orders data using the `bin/magento saas:resync --feed orders` command. The error was resolved by updating the Channel Manager package dependencies for the Sales Data Exporter module, which was renamed from `magento/module-sales-data-exporter` to `magento/module-sales-orders-data-exporter`.

## v1.0.0

Initial release, compatible with the following Commerce versions:

* Open Source (CE): 2.4.x
* Adobe Commerce (EE): 2.4.x
* Adobe Commerce for Cloud (ECE): 2.4.x
* Stability: Stable
