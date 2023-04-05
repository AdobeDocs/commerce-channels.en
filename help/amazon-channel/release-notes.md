---
title: '[!DNL Amazon Sales Channel] Release Notes'
description: Review the release notes for information about all [!DNL Amazon Sales Channel] releases.
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
---
# Release Notes

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] can be installed on instances with Magento Open Source, Adobe Commerce, and Adobe Commerce on cloud infrastructure versions 2.3.x and 2.4.x. The extension is no longer supported on Adobe Commerce 2.1, Magento Open Source 2.2, or Magento 1.
> <br>Support is available for [!DNL Amazon sales channel]  versions 4.0.0 and 4.1.0 on Adobe Commerce 2.3.x versions only.
> <br>[!DNL Amazon sales channel] version 4.2.0+ is compatible with Adobe Commerce 2.3.x versions, but support is available only for Adobe Commerce 2.4.x versions.
>

These release notes describe the initial release of [!DNL Amazon sales channel] and include:

![New](../assets/new.svg) New features
![Fixed issue](../assets/fix.svg) Fixes and improvements
![Known issue](../assets/bug.svg) Known issues

See [Upcoming Releases](https://devdocs.magento.com/release/){target="_blank"} for versioning, support, and compatibility.

## v4.4.4

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x and 2.4.0 (supported for 2.4.1 and newer)

![Fixed issue](../assets/fix.svg) Added support for Adobe Commerce 2.4.6 and PHP 8.2.

![Fixed issue](../assets/fix.svg) Reduced noise in logs.

![Fixed issue](../assets/fix.svg) Improved stability of pulling updates.

![Fixed issue](../assets/fix.svg) Simplified the process for running single action-like pull or for applying from CLI.

![Fixed issue](../assets/fix.svg) Upgraded the dependency for `magento/services-connector`.

![Fixed issue](../assets/fix.svg) Fixed sync issues in UK accounts with invalid country code.

![Fixed issue](../assets/fix.svg) Hardcoded the entity_type_id for catalog product entity causes issues with Magento Price Source.

![Fixed issue](../assets/fix.svg) Corrected an issue preventing accounts that are deleted on a backend from another instance from deleting from the UI as well.

![Fixed issue](../assets/fix.svg) Fixed an issue with some cart rules breaking order import.

## v4.4.3

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x and 2.4.0 (supported for 2.4.1 and newer)

![Fix](../assets/fix.svg) Added support for Adobe Commerce 2.4.4.

## v4.4.2

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x and 2.4.0 (supported for 2.4.1 and newer)

![Fix](../assets/fix.svg) Updated dependencies to support other updated extensions.
![Fix](../assets/fix.svg) Added support for PHP 8.1.

## v4.4.1

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x and 2.4.0 (supported for 2.4.1 and newer)

![Fix](../assets/fix.svg) Changed the way Adobe Commerce receives the _User Name_ field from Amazon. Previously, there was an error during order creation when the _User Name_ field contained special characters. Adobe Commerce now receives the _User Name_ data and filters out the special characters so the order can be created successfully.

## v4.4.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x and 2.4.0 (supported for 2.4.1 and newer)

![New](../assets/new.svg) Added support for Read-Only Mode to the configuration. See [sales channel settings](sales-channel-settings.md).

![Fix](../assets/fix.svg) Changed the data flow so that multiple copies of the same instance can fetch updates simultaneously.

![Fix](../assets/fix.svg) Changed the sync process for syncing account information. Added a cron job to sync with remote account and added the same functionality to the CLI commands.

![Fix](../assets/fix.svg) Added CLI command arguments and flags for more precise control.

![Fix](../assets/fix.svg) Corrected the Background Tasks (cron) Source in the system configuration.

![Fix](../assets/fix.svg) Corrected the issue preventing the creation of orders when the country code was set to Puerto Rico (PR).

## v4.3.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x and 2.4.0 (supported for 2.4.1 and newer)

![Fix](../assets/fix.svg) <!--CHAN-xxxx-->The _Order Details_ feature has been redesigned and no longer relies on the _Import Orders_ setting. Order details now appear in the Amazon Sales Channel interface for all orders.

![Fix](../assets/fix.svg) In the _[!UICONTROL Marketing]_ menu in the Admin, the name has been changed from _[!UICONTROL Amazon]_ to _[!UICONTROL Amazon Sales Channel]_.

![Known issue](../assets/bug.svg) **Important**: Known issues with Adobe Commerce 2.4.0 compatibility are resolved in the Adobe Commerce 2.4.1 release.

- Amazon cron processes in `error` state
- Installation with Commerce 2.4.0 fails when creating stores in the database
- Creating product fails when MSI is installed

## v4.2.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x (supported for 2.4.x)

If you have a previous [!DNL Amazon sales channel] version installed and attempt to update your Adobe Commerce to version 2.4.0, you are prompted to update the extension before you can complete the Adobe Commerce update.

![Known issue](../assets/bug.svg) When [!DNL Amazon sales channel] 4.2.0 is integrated with version 2.4.0 and [Inventory Management](https://docs.magento.com/user-guide/catalog/inventory.html) is enabled, there is a known issue that prevents the addition of products in your Commerce catalog. This issue will be addressed in a future Commerce release.

![New](../assets/new.svg) [!DNL Amazon sales channel] has been enhanced to accept text-based address data and match it to standardized address formats, including city, state, and zip code. This update enables order and shipping data to synchronize (sync) with Amazon without address errors.<br/>For example, a shopper inputs the city, state, zip code as `Escondido, californiA 92025-1501`. Amazon Sales Channel imports and matches the data to the standard format as `Escondido, CA 92025`, and then syncs it back to Amazon in this standardized format.

![New](../assets/new.svg) Added support for PHP 7.4.

![New](../assets/new.svg) <!--CHAN-4334-->Added support for Adobe Commerce 2.4.x. Previous versions may be compatible with Commerce 2.4.x, but are not supported. See [Upcoming releases](https://devdocs.magento.com/release/){:target="_blank"} for version compatibility. Amazon Sales Channel must be updated to 4.2.0 before the Adobe Commerce 2.4.0 update can be completed.

![Fix](../assets/fix.svg) <!--CHAN-4431-->Corrected an issue that caused an _Access Denied_ error for UK customers.

![Fix](../assets/fix.svg) <!--CHAN-4394-->Corrected an issue that prevented the Amazon shipping status from syncing to the corresponding Commerce order, thus "locking" the order's shipping status as `Pending` in Commerce and `Unshipped` in Amazon. With the new standardized address feature, these shipping status errors have been resolved.

![Fix](../assets/fix.svg) <!--ticket#-->Updated order synchronization (sync) to ignore failed order imports, thus reducing multiple sync attempts and allowing subsequent imports to process, with order sync requests submitted every five minutes. Sync errors are still recorded in the error log, but marked as "processed" to allow further logging functions. Also, [!DNL Amazon sales channel] now automatically removes excess data collected for orders that fail to create in Commerce.

![Fix](../assets/fix.svg) Updated error logging to collect more information for uncaught exception and extension update errors.

![Fix](../assets/fix.svg) <!--ticket#-->Corrected an issue that caused the initial sync of the _lowest price_ data to fail due to a missing _price_ value.

![Fix](../assets/fix.svg) <!--CHAN-4410-->Corrected issues that caused filtering errors in the _Amazon orders_ view when the date range field is left blank.

![Fix](../assets/fix.svg) <!--CHAN-4439-->Corrected an issue that caused quantity-related stock and fulfillment sync errors. The extension now rounds down quantity values entered as a decimal before syncing with Amazon.<br/> For example, when a merchant manually inputs a quantity of `2.5`, the extension rounds down the value to `2` and then syncs the updated quantity with Amazon.

## v4.1.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.x

![New](../assets/new.svg) <!--4247, 4230-->Changed the order import process to align with Commerce order requirements. These changes correct issues that prevented Commerce from creating the corresponding order for an imported order. See [Manage Orders](managing-orders.md) for information on order blockers and solutions.

![New](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->Updated the _Recent Orders_ section of the store dashboard and added a new _All Orders_ view that shows all your Amazon orders, including filter options and pagination for viewing more orders. See [Amazon Store Dashboard](amazon-store-dashboard.md) and [View Amazon Orders](amazon-orders-all.md).

![New](../assets/new.svg) Added the _[!UICONTROL Order Notes]_ column of the redesigned _[!UICONTROL Amazon Orders]_ table in both _[!UICONTROL Recent Orders]_ and _[!UICONTROL All Orders]_ views. _[!UICONTROL Order Notes]_ let the merchant know there is an issue with the order's import. See [View Amazon Orders](amazon-orders-all.md).

![New](../assets/new.svg) <!--CHAN-4013-->Updated product condition parameters to align with the [Amazon Renewed](https://sell.amazon.com/programs/renewed) program. See [Renewed Products](renewed-products.md).

![New](../assets/new.svg) <!--CHAN-3680-->Updated [Amazon Order Details](amazon-order-details.md) to include "generic data" for orders that are fulfilled by Amazon. See [Fulfilled by](fulfilled-by.md).

![Fix](../assets/fix.svg) <!--CHAN-4069-->Corrected an issue causing the distortion of icons on the store card.

![Fix](../assets/fix.svg) <!--CHAN-4165-->Corrected an error preventing the _Login_ screen from appearing after the session times out.

![Fix](../assets/fix.svg) <!--CHAN-4211-->Corrected an issue preventing the Amazon order tax amount from importing into the new Commerce order.

![Fix](../assets/fix.svg) <!--CHAN-4234-->Corrected an issue that caused revenue totals displayed on the store dashboard to include orders in `Canceled` or `Error` status.

![Fix](../assets/fix.svg) <!--CHAN-4326-->Corrected an issue that caused order import errors associated with third-party extensions that use _Magento Shipping_ methods to create orders.

![Fix](../assets/fix.svg) <!--CHAN-4357-->Corrected an issue that caused errors when running cron synchronization. A lock has been added on the CLI command that prevents two cron jobs from synchronizing at the same time.

![Fix](../assets/fix.svg) Updated content security policy for support with Commerce version 2.3.5.

## v4.0.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.3.0-2.3.4

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0 is not supported for Adobe Commerce 2.3.5. For support with Adobe Commerce 2.3.5, upgrade to Amazon Sales Channel 4.1.0.

![New](../assets/new.svg) Introduced a new [Amazon Sales Channel](amazon-sales-channel-home.md) home page with improved "card view" for your store information.

![New](../assets/new.svg) Introduced a new [store dashboard](amazon-store-dashboard.md) with listing, recent orders, and store setting information.

![New](../assets/new.svg) Introduced a simpler, streamlined [onboarding process](amazon-onboarding-home.md) and [default store settings](default-store-settings.md) to get your stores integrated faster.

![Known issue](../assets/bug.svg) <!--CHAN-4102--> When [creating attributes](managing-attributes.md) for importing images from listings and **Store Views** is set to `All Store Views (Global)`, a known issue exists preventing images from importing to all store views. If you change the setting for **Store Views (to import values into)** to a specific store, the images import for that store.

## v3.0.1

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.2.4 and newer

![Fix](../assets/fix.svg) **Numerical Field Settings**: <!--CHAN-3779-->Fields that require a numeric-based value have been updated to only accept numeric characters. Example: Pricing Rule Settings > Adjustment Amount field

![Fix](../assets/fix.svg) **User Guide Links**: <!--CHAN-3778-->Incorrect _User Guide_ links have been corrected.

![Fix](../assets/fix.svg) **Duplicate Amazon Listings**: <!--CHAN-3593-->A previously reported issue that cause duplicate Amazon listings is now corrected. Prior to this release, the extension added the Country Code for the Amazon region to SKU values when importing listings. The listing matched with the catalog item, but the extension created a new, duplicate listing with the appended SKU. With this release, the extension does not modify the SKU for imported listings, and no changes are made to existing listings. You can use the [!UICONTROL End Listing(s)] on Amazon option to remove duplicate listings.

## v3.0.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.2.4 and newer

![New](../assets/new.svg) **Amazon UK Marketplace Now Available**: Users can choose the United Kingdom marketplace when creating and integrating a Commerce store. This UK upgrade includes additional support for:

- [Amazon VAT Calculation Service](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [Product Tax Code](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&language=en_US){target="_blank"} information.

![New](../assets/new.svg) **Improved Logging**: <!--CHAN-3642, 3672-->Implemented the **Enable Debug Logging** feature to collect additional synchronization data when troubleshooting is needed. See the [Sales Channels Settings](https://docs.magento.com/user-guide/configuration/sales-channels/global-settings.html) topic in the Configuration Reference.

![Fix](../assets/fix.svg) **Product Catalog**: <!--CHAN-3687-->Corrected an issue that prevented images imported with an Amazon listing from being applied to the corresponding Commerce catalog product.

![Fix](../assets/fix.svg) **Order Creation**: <!--CHAN-3708-->Corrected an issue preventing Commerce from creating orders for an Amazon order that does not match with a Commerce catalog product.

![Known issue](../assets/bug.svg) **Duplicate Amazon Listings**: <!--CHAN-3593-->This issue causes the catalog to create an item for an imported listing, using the same SKU but with a region code added on the end. Amazon then processes the modified SKU as a new item and creates a listing. This issue will be addressed in a future release.

## v2.0.0

[!BADGE Compatibility]{type=Informative tooltip="Compatibility"} Adobe Commerce versions 2.2.4 and newer

>[!NOTE]
>
>Version 1.0.0 was available in limited release only.

![New](../assets/new.svg)  **Simplified Onboarding and Maintenance**: Add and integrate with your Amazon Seller account through a step-by-step process with detailed instructions available through the Admin. Maintain your stores, accounts, and listed products through one dashboard.

![New](../assets/new.svg)  **Multiple Account Support**: Manage and monitor multiple Amazon brands and marketplace regions through the Admin.

![New](../assets/new.svg)  **Intelligent Pricing**: Set automated repricing rules to increase your chances for the coveted Buy Box. Set prices to dynamically adjust to the current Buy Box price, or lowest competitor pricing. Set limits to repricing to protect your margin.

![New](../assets/new.svg)  **Listing Management**: Automate product listings and sync your Commerce catalog to the Amazon Marketplace using listing rules. Add specific overrides to finely control your offerings. Monitor and manage all your listings directly from the Admin.

![New](../assets/new.svg)  **Consistent Inventory Management**: Keep your Commerce and Amazon inventory quantities in constant synchronization.

![New](../assets/new.svg)  **Order and Fulfillment Management**: Track Amazon orders through the dashboard, with seamless communication and inventory updates. Complete and track order shipments as fulfilled by Amazon, merchant fulfilled, or a mix of methods.

![Known issue](../assets/bug.svg)  You may encounter longer wait times to update product quantities. Updates for product quantity may take ~two hours to sync.

![Known issue](../assets/bug.svg)  Imported orders may have a type of _Prime_ or _Premium_ orders. You should verify these orders in your Amazon Seller Account.

![Known issue](../assets/bug.svg)  Ineligible bundled products may display as Eligible for listing on Amazon. One of the products within the bundled product may not be eligible. If you encounter issues, check the eligibility status for bundled products items.

![Known issue](../assets/bug.svg)  When using Inventory Management for Commerce 2.3.x, a partial stock reindex may not trigger when an order is created. The salable quantity recalculates hourly, which may cause overselling during this update interval.
