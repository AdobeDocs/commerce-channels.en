---
title: View Amazon attribute mapping
description: Verify values for your linked Commerce attributes to correctly sync between Commerce and Amazon.
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
---
# View Amazon attribute mapping

As you map Amazon attributes to [!DNL Commerce] attributes, Amazon sales channel tracks and provides a filterable list of all Amazon values. Use this page to verify values for your linked [!DNL Commerce] attributes correctly sync between [!DNL Commerce] and Amazon. You can review synced values for Amazon attribute linked or not linked to a [!DNL Commerce] attribute. To create or edit your Amazon attributes, see [Creating and Editing Attributes](./creating-attributes.md).

The _Amazon Value_ differs depending on the attribute type and the Amazon attribute that you view. For example, a listed Amazon value for `Label` would be a text value while `AmazonListPrice` would be a numerical amount. The status indicates if the Amazon value has been imported.

## View your attribute values

1. On the _[!UICONTROL Admin]_ sidebar, go to **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Click **[!UICONTROL Attributes]** in the left-side menu, locate an Amazon attribute, and click either **[!UICONTROL Create]** or **[!UICONTROL Edit]** in the _[!UICONTROL Action]_ column.

1. Click the **[!UICONTROL Matching Attribute Values]** tab.

    Listings that have a corresponding [!DNL Commerce] catalog product show a linked value in the _[!UICONTROL Magento Product SKU]_ column. Clicking a link opens the corresponding catalog product detail page. Changes to Amazon attributes on the product detail page do not sync back to Amazon sales channel.

>[!TIP]
>To edit or assign the mapping for a listing to a catalog product, see [Update Required Info](./amazon-manually-update-incomplete-listing.md).

![View attribute values](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| Field                            | Description                                                                                                                                                                                                                                                                                                                            |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region]              | The region for sales activity defined in **[!DNL Amazon Marketplace] Country** during store integration.                                                                                                                                                                                                                               |
| [!UICONTROL Magento Product SKU] | Indicates the [!DNL Commerce] products synced with the Amazon store. The value is a product ID assigned by [!DNL Commerce] and linked to a product in the catalog. To open the product in [!DNL Commerce], click the link.                                                                                                             |
| [!UICONTROL ASIN]                | Indicates the Amazon Standard Identification Number (ASIN) 10-character alphanumeric unique identifier assigned to the product by Amazon for product identification.                                                                                                                                                                   |
| [!UICONTROL Amazon Value]        | Indicates the value for the selected attribute. The Amazon Value differs depending on the attribute type and the Amazon attribute that you view. For example, a listed Amazon value for `Label` would be a text value while `AmazonListPrice` would be a numerical amount. The status indicates if the Amazon value has been imported. |
| [!UICONTROL Status]              | Indicates if the attribute values have been imported into [!DNL Commerce] and linked to a [!DNL Commerce] attribute. Options: `Not Imported` / `Imported`                                                                                                                                                                              |
