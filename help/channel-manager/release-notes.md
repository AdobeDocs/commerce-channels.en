---
title: '[!DNLChannel Manager] Release Notes'
description: The latest release information for [!DNL Channel Manager] from Adobe Commerce.
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
---
# [!DNL Channel Manager] Release Notes

These release notes describe the initial release of [!DNL Channel Manager] and include:

![New](../assets/new.svg) New features
![Fixed issue](../assets/fix.svg) Fixes and improvements
![Known issue](../assets/bug.svg) Known issues


## v2.0.0

<table>
<tr style="border: 0;">
  <td>
    <i>March TBD, 2023</i><br>
    [!BADGE Compatibility]{type=Informative tooltip="Compatibility"}<br>Adobe Commerce versions 2.4.0 - 2.4.6
  </td>
  </tr>
  </table>
  
  ![New](../assets/new.svg)<!--CHAN-5204--> Added PHP 8.2 support
  
  
## v1.1.0

<table >
<tr style="border: 0;">
  <td>
    <i>November 23, 2022</i><br>
    [!BADGE Compatibility]{type=Informative tooltip="Compatibility"}<br>Adobe Commerce versions 2.4.0 - 2.4.5
  </td>
  </tr>
</table>
  
![New](../assets/new.svg)<!--CHAN-5204--> **Returns and Refunds**—You can now process Walmart Marketplace returns and refunds process for orders shipped through an Adobe Commerce and Magento Open Source Channel Manger store. Information and updates about returns and refunds are synchronized between Walmart and Adobe Commerce so that the current data is available in both the [!DNL Commerce] storefront and [!DNL Walmart Marketplace]. See [Return and refund orders](return-refund-orders.md).

![Fixed](../assets/fix.svg)<!--CHAN-5661--> Fixed the `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` error that occurred when resynchronizing Channel Manager orders data using the `bin/magento saas:resync --feed orders` command. The error was resolved by updating the Channel Manager package dependencies for the Sales Data Exporter module, which was renamed from `magento/module-sales-data-exporter` to `magento/module-sales-orders-data-exporter`.

## v1.0.0

<table>
<tr style="border: 0;">
  <td>
    <i>January 14, 2022</i><br>
    [!BADGE Compatibility]{type=Informative tooltip="Compatibility"}<br>Adobe Commerce versions 2.4.0 - 2.4.5
  </td>
  </tr>
</table>

