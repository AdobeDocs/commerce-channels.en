---
title: Add Products to Channel Manager
description: 'Create product assortment for [!DNL Walmart Marketplace] sales by adding products from the catalog to the sales channel configured in Channel Manager.' 
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
---

# Add Products to [!DNL Channel Manager]

To add products to the [!DNL Walmart Marketplace] sales channel, select them from the [!DNL Commerce] product catalog and import them to [!DNL Channel Manager].
The import process can take up to 30 minutes or more depending on how many products you select.

## Prerequisite

**[Map catalog attributes](map-catalog-attributes.md)**—In the [!DNL Channel Settings] configuration, map at least one attribute from the [!DNL Commerce] product catalog to one of the required Walmart Product Identifiers—–GTIN, ISBN, ISSN, UPC, EAN.

## Listing requirements

[!DNL Commerce] product listings must have the following required attribute configuration:

- **[!UICONTROL Connect to Channel Manager]** attribute is enabled

- Provide valid values for the required Walmart attributes.

  - At least one product attribute that matches one of the required [!DNL Walmart Marketplace] product identifiers–GTIN, ISBN, ISSN, UPC, EAN.

  - Product price specified to a maximum of two decimal places, for example `9.99`

  - Product weight specified to a maximum of two decimal places, for example `1.25`

>[!TIP]
>
>For additional information about optimizing listings for your sales channel, see the [Walmart Marketplace Listing Quality Optimization Guide](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## Add products

1. From a connected sales channel store, select **Add products** to open the product catalog.

   ![Add products to sales channel store](assets/add-initial-products-to-connected-channel.png)

   The catalog opens in a new tab.

1. From the catalog product grid, select products to sell on [!DNL Walmart Marketplace].

   ![Send products to the sales channel store](assets/select-products-from-catalog.png)

1. Enable the **[!UICONTROL Connect to Channel Manager]** attribute for the selected items.

   - From **[!UICONTROL Actions]**, select **[!UICONTROL Update attributes]**.

   - Scroll to the **[!UICONTROL Connect to Channel Manager]** attribute and enable it.

   - Verify that the product attributes include at least one of the required [!DNL Walmart Product IDs].

   - Select **[!UICONTROL Save]**.

     A confirmation message displays.

     ![Product import from catalog to sales channel confirmation message](assets/product-import-from-catalog-confirmation.png)

     If the message indicates that the update is scheduled, use the [queue:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] command to process the update immediately.

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. After the import operation completes, verify the products that you added by returning to [!DNL Channel Manager] and selecting **[!UICONTROL Listings]**.

   Initially, the products are in *Draft* status. Select **[!UICONTROL Refresh products]** to update the table.

1. Update the view to show the new products added to Channel Manager by selecting the **[!UICONTROL Draft]** status card.

   ![Products imported to connected sales channel](assets/products-in-marketplace-sales-channel.png)


