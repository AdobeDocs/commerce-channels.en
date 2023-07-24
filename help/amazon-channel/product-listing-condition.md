---
title: Amazon sales channel - Product listing condition
description: Use the Product Listing Condition settings to map your Commerce products to an Amazon product condition, such as "New" or "Refurbished".
feature: Sales Channels, Products, Merchandising
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
---
# Product listing condition

Product listing condition settings are part of your store listing settings. You can access the listing settings on the [store dashboard](./amazon-store-dashboard.md).

Amazon requires a product listing to have a defined condition. If all your products are the same condition, you can select one of the Amazon condition options to represent all of your products as your global condition value. Standard Amazon conditions include:

- `New`
- `Refurbished`
- `Used; Like New`
- `Used; Very Good`
- `Used; Good`
- `Used; Acceptable`
- `Collectible; Like New`
- `Collectible; Very Good`
- `Collectible; Good`
- `Collectible; Acceptable`

>[!IMPORTANT]
>
>If you sell renewed (refurbished) products, you must enroll in the [!DNL Amazon Renewed Program]. See [Renewed Products](./renewed-products.md).

However, if your catalog contains products in different conditions (such as New, Used, and Refurbished), you must choose **[!UICONTROL Assign Condition Using Product Attribute]**. This setting allows you to map your [!DNL Commerce] condition attribute and values to your Amazon listing's conditions.

During [Pre-setup tasks](./amazon-pre-setup-tasks.md), you are encouraged to create a [!DNL Commerce] product attribute for a product's condition. If you offer products in various conditions and you have not created a condition attribute, see [Create a product attribute in [!DNL Commerce]](./ob-creating-magento-attributes.md). After the condition attribute is created, you can assign a condition value to each of your products in your [!DNL Commerce] catalog.

## Configure settings

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the **[!UICONTROL Product Listing Condition]** section.

1. For **[!UICONTROL Listing Product Condition]**, choose an option.

    Choose one of the standard Amazon conditions for your global condition value for all of your listings. Default setting is `New`.

    If you have products/listings that have different conditions, choose `Assign Condition Using Product Attribute` to define your product condition settings in the additional fields that appear.

1. For **Condition Attribute**, choose the [!DNL Commerce] attribute to map values for each of the standard Amazon condition attributes.

   If you have products in the `Used` or `Collectible` condition but you do not distinguish further, you can map to a single `Used` or `Collectible` Amazon condition and leave the others blank. This method maps all of your `Used` or `Collectible` conditions to the single Amazon Used or Collectible condition.

   For example, you have a single `Used` condition for your products. When mapping, you choose whether you want to map to the Amazon condition `Used; Like New`, `Used; Very Good`, `Used; Good`, or `Used; Acceptable`. Only complete the field for the Amazon condition you want, leaving the other `Used` options set to `--Select Option--`. In the example image, all [!DNL Commerce] products in `Used` condition are mapped to the Amazon `Used; Very Good` condition.

   You can also enter descriptive text for your conditions, except `New`.

1. When complete, click **[!UICONTROL Save listing settings]**.

![Product listing condition](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| Field                                    | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Listing Product Condition]   | The condition of your product listings. Options: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>If you sell a single product condition, choose one of the standard Amazon conditions. If your [!DNL Commerce] catalog contains products in various conditions, choose `Assign Condition Using Product Attribute`.            |
| [!UICONTROL Condition Attribute]         | The [!DNL Commerce] attribute that defines the condition for your products. Select the Magneto attribute you created to map to the Amazon condition attribute. In the [Pre-Setup Tasks example](./ob-creating-magento-attributes.md) recommends naming it as `Amazon Condition`. When chosen, additional fields appear for mapping the standard Amazon conditions.                                                                                                                                                                        |
| [!UICONTROL Additional Condition fields] | For each of the standard Amazon conditions, choose the corresponding condition. The options are the condition labels you added when you [created your Amazon condition attribute](./ob-creating-magento-attributes.md).<br><br>If you have products in the `Used` or `Collectible` condition but you do not distinguish further, you can map to a single `Used` or `Collectible` Amazon condition and leave the others blank. This method maps all `Used` or `Collectible` conditions to the single Amazon Used or Collectible condition. |

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
