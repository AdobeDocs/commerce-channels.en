---
title: Attributes for Amazon listings
description: Amazon Sales Channel provides the [!UICONTROL Attributes] tab to monitor the list of Amazon and Commerce attributes and how they are mapped for product matching.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
---
# Attributes for Amazon listings

The _[!UICONTROL Attributes]_ view shows your list of Amazon and [!DNL Commerce] attributes. The list also indicates attributes that have been mapped for product matching. For more information, see [Manage Attributes](./managing-attributes.md).

![Attributes view](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

From the _[!UICONTROL Attributes]_ view, you and review your attribute settings in the table and [create or edit](./creating-attributes.md) an attribute.

## View your attributes list

1. On the _Admin_ sidebar, go to **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. Click **[!UICONTROL Attributes]** in the left-side menu, locate an Amazon attribute, and review your attribute list.

1. Create or edit an attribute, as needed:

   - To [create](./creating-attributes.md#create-an-attribute) and define Matching Attribute Values for the attribute, click **[!UICONTROL Create]**.

   - To deactivate or [edit the settings](./creating-attributes.md#edit-an-attribute) or Matching Attribute Values for the attribute, click **[!UICONTROL Edit]**.

      Editing an attribute includes changing the attribute mapping for product matching.

| Field                                       | Description                                                                                                                                                                                                                                                                                                                                                                                                         |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country]                        | The country for sales activity defined in  **[!DNL Amazon Marketplace] Country** during [store integration](./store-integration.md).                                                                                                                                                                                                                                                                                |
| [!UICONTROL ID]                             | Generic attribute value generated by [!DNL Commerce] when the attribute is created.                                                                                                                                                                                                                                                                                                                                 |
| [!UICONTROL Amazon Attribute Name]          | The name of the attribute imported from Amazon.                                                                                                                                                                                                                                                                                                                                                                     |
| [!UICONTROL Product Catalog Attribute Code] | If mapped, the [!DNL Commerce] attribute assigned to map to the _[!UICONTROL Amazon Attribute Name]_ for matching catalog and listing products.                                                                                                                                                                                                                                                                     |
| [!UICONTROL Overwrite Magento Values]       | If the attribute is set to `Overwrite Existing Magento Values` in the Attribute Settings, the table shows `Enabled`. Enabled means that when updated product information for the attribute is received from Amazon, the new information updates (overwrites) the corresponding information for the product in your [!DNL Commerce] catalog. It can also affect your products listed in your [!DNL Commerce] stores. |
| Status                                      | Indicates if the attribute values have been imported into [!DNL Commerce] and mapped to a [!DNL Commerce] attribute. Options: `Enabled` / `Disabled`                                                                                                                                                                                                                                                                |
| Action                                      | Indicates the task options available for the attribute. Options: `Create` / `Edit`                                                                                                                                                                                                                                                                                                                                  |
