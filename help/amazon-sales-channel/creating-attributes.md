---
title: Create and Edit Attributes
description: Amazon Sales Channel provides the Attributes view to help you review the current Amazon attributes and linked Commerce attributes.
---

# Create and edit attributes

Create or update [!DNL Commerce] attributes as you sell through Amazon and update your stores. Review the current Amazon attributes and linked [!DNL Commerce] attributes through the [_Attributes_ view](./attributes-view.md) of the [!DNL Amazon Sales Channel] home page. The _Action_ column shows the available actions for the attribute. You can either create and map a new [!DNL Commerce] attribute for an unlinked Amazon attribute, or you can edit an existing [!DNL Commerce] attribute and its mapping to an Amazon attribute.

As you create and update attributes, you may want to verify the attribute values for [!DNL Commerce] and Amazon products. These values may differ if you do not sync and import values from Amazon. To review Amazon values for these attributes, see [Reviewing Amazon Attribute Mapping](./amazon-matching-attributes-values.md). If you want to change those values, you can [edit or create a mapping](./amazon-manually-update-incomplete-listing.md) between Amazon and [!DNL Commerce].

## Create an attribute {#create-an-attribute}

These steps create a [!DNL Commerce] attribute and map it to an Amazon attribute. Depending on configurations, the values may start syncing between catalogs.

1. On the _Admin_ sidebar, go to **Marketing** > _Channels_ > **Amazon Sales Channel**.

1. Click **Attributes** in the left-side menu, locate an Amazon attribute, and click **Create Attribute** in the _Action_ column.

1. To enable the syncing of the Amazon values to the linked [!DNL Commerce] attribute, set **Is Active** to `Yes`.

    When set to `Yes`, the values sync according to your configuration.

1. Choose `Create New Magento Attribute` for **Select Magento Product Attribute**.

    The attribute maps to the chosen for **Amazon Attribute Name**.

1. Enter a **Magento Product Attribute Name**.

1. Enter a **Magento Product Attribute Code**.

    This value must be all lowercase without spaces.

1. For **Attribute Set Ids**, choose an Attribute Set to assign.

   Typically, attributes are a part of an attribute set, such as a set for colors having attributes for blue, green, yellow, and red.

1. For **Type**, choose the type of the attribute value, such as text and numbers.

    This option affects the allowed value for the attribute.

1. For **Use for Promo Rule Conditions**, set to `Yes` to allow the attribute to be available for a parameter within your promotional conditions.

1. For **Used in Search**, set to `Yes` if the attribute and value can be used in product searches.

1. For **Comparable on Storefront**, set to `Yes` if the attribute value can be used in Amazon's "Compare By" functionality.

1. Choose the [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target="_blank"} for the attribute, and then select one or more Store Views to import Amazon values into.

    If the scope is set to `Global`, the _Store View_ cannot be changed after the attribute is created.

    If you choose `All Store Views (Global)`, it syncs and saves values to all of your Amazon store views. You may only want to sync values to specific store views.

1. When complete, click **[!UICONTROL Save Attribute Settings]**.

After saving, you may want to edit the attribute to review settings and matching Amazon and [!DNL Commerce] values for the attribute. You can also indicate if Amazon values should overwrite [!DNL Commerce] values.

![create attribute settings](assets/amazon-attribute-settings-create.png)

|Field|Description|
|--- |--- |
|Is Active|Indicates if this attribute is live and actively syncs between Amazon and [!DNL Commerce]. Set to `Yes` to ensure the attribute values from Amazon and [!DNL Commerce] stay in sync for the selected attribute.|
|Select Magento Product Attribute|Indicates the selected attribute that you want linked to the listed Amazon Attribute Name. When creating an attribute, choose `Create New Magento Attribute`.|
|Amazon Attribute Name|Shows the name of the Amazon attribute you chose. The selected attribute links to this Amazon attribute. You cannot edit this value through [!DNL Commerce].|
|Magento Product Attribute Name|Indicates the attribute name or "label".|
|Magento Product Attribute Code|Indicates the attribute code, all in lowercase characters without spaces.|
|Attribute Set Ids|Indicates the Attribute Set to assign the attribute to. Attributes tend to be part of an attribute set, such as a set for colors having attributes for blue, green, yellow, and red.|
|Type|Indicates the value type of the attribute value, such as text and numbers. The selection affects the allowed value for the attribute.|
|Use for Promo Rule Conditions|Toggle to `Yes` to allow the attribute to be available for a parameter within your promotional conditions.|
|Used in Search|Indicates if the attribute and value can be used in product searches.|
|Comparable on Storefront|Indicates if the attribute value can be used in Amazon's "Compare By" functionality.|
|Magento Product Attribute Scope|Indicates the [scope](https://docs.magento.com/user-guide/configuration/scope.html){target="_blank"} for the attribute. Options: Global / Store View<br>When set to `Global`, the Store View cannot be edited after the attribute is created.|
|Store Views (to import values into to)|Only appears when scope is set to `Store View`. Choose the [store view](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} to which the Amazon attribute values are synced. Choosing `All Store Views (Global)` updates the value across all [!DNL Commerce] store views.|

## Edit an attribute {#edit-an-attribute}

1. On the _Admin_ sidebar, go to **Marketing** > _Channels_ > **Amazon Sales Channel**.

1. Click **Attributes** in the left-side menu, locate an Amazon attribute, and click **Edit** in the _Action_ column.

1. To enable or disable the syncing of the Amazon values to the linked [!DNL Commerce] attribute, set **Is Active** to `Yes` or `No`.

    When set to `Yes`, the values sync according to your configuration.

1. For **Select Magento Product Attribute**, verify or update the attribute to map to the chosen **Amazon Attribute Name**.

1. Indicate if you want the incoming Amazon attribute value to overwrite existing attribute value.

    For example, you may not want to overwrite the prices from Amazon into [!DNL Commerce].

    - **Do Not Overwrite Existing Magento Values** - Retains the value, keeping different values for your [!DNL Commerce] and Amazon stores.

    - **Overwrite Existing Magento Values** - Overwrites the value in the [!DNL Commerce] product catalog with the incoming Amazon value.

1. If available for edit, choose one or more **Store Views (to import Amazon values into)**.

    If the attribute was created with a `Global` scope, the _Store View_ cannot be changed after the attribute is created.

    If you choose `All Store Views (Global)`, it syncs and saves values to all store views. You may only want to sync values to specific store views.

1. When complete, click **[!UICONTROL Save Attribute Settings]**.

![edit attribute settings](assets/amazon-attribute-settings-edit.png)

|Field|Description|
|--- |--- |
|Is Active|Indicates if this attribute is live and actively syncs between Amazon and [!DNL Commerce]. Set to `Yes` to ensure the attribute values from Amazon and [!DNL Commerce] stay in sync for the selected attribute.|
|Select Magento Product Attribute|Indicates the selected [!DNL Commerce] attribute that you want linked to the listed Amazon Attribute Name. If you want to change the linked [!DNL Commerce] attribute, choose a different attribute from the drop-down list. Values sync according to configurations.|
|Amazon Attribute Name|Shows the name of the Amazon attribute as defined in [!DNL Amazon Seller Central]. The selected [!DNL Commerce] attribute links to this Amazon attribute. You cannot edit this value through [!DNL Commerce].|
|Overwrite Existing Value|Indicates if the Amazon attribute values overwrite existing [!DNL Commerce] values, affecting all products with this [!DNL Commerce] attribute.<ul><li>**Do Not Overwrite Existing Magento Values** - (Default) Retains the [!DNL Commerce] value, keeping different values for [!DNL Commerce] and Amazon stores.</li><li>**Overwrite Existing Magento Values** - Saves the Amazon value over the [!DNL Commerce] value in the [!DNL Commerce] product catalog.</li></ul>|
|Magento Product Attribute Scope|Does not appear when editing an attribute if the attribute was created with the `Global` scope. Indicates the [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target="_blank"} was created and set to `Store View`.|
|Store Views (to import values into to)|Choose your [!DNL Commerce] [store view](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} to which to sync the Amazon attribute values. Choosing `All Store Views (Global)` updates the value across all store views.|
