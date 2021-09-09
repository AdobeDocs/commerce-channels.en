---
title: Overrides
description: Amazon Sales Channel provides the Overrides tab to help you identify and manage how you are applying overrides in your Amazon listings.
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
---
# Overrides

The _[!UICONTROL Overrides]_ tab shows your Amazon listings to which you have applied an override. An override is a listing-specific setting that can be used set a defined value to a listing. An override applied to a listing defines the setting for the listing, regardless of other defined listing settings or rules for which the listing is eligible. When an override is applied to a listing, the listing appears on the _[!UICONTROL Overrides]_ tab. The value defined in the override appears in the appropriate column for the listing. There are four types of overrides that can be applied: Price, Handling Time, Condition, and Seller Notes.

## Types of overrides

|Type|Description|
|---|---|
|Price|An override that sets the price of the listing, ignoring all other price settings for the listing. <br><br>**Example**: You have defined a 20% discount price rule that applies to all products in a specific category of your catalog. You have a product that is new to market and demand is high, so you do not want the discounted price applied to the listing even though the product is in that category. You can select the listing, [create a price override](./creating-editing-overrides.md#edit-override-single-listing), and define the listing price in a price override. |
|Handling Time|An override that sets the handling time for a listing, ignoring the default handling time set in listing settings.<br><br>**Example**: Your default handling time for your listings is set to 2 days. You have a product that is fragile and requires an extra day to ensure its special packaging for shipping. You can view the listing, [create a handling time override](./creating-editing-overrides.md#edit-override-single-listing), and define the handling time at three days.<br><br>**Note:** Not available for products set to `Fulfilled by Amazon`. |
|Condition|An override that sets the condition value of a listing, regardless of the condition attribute assigned to the listing.<br><br>**Example**: Most of the products in your catalog are New condition, but you have a product that is in Refurbished condition. You can view the listing, [create a condition override](./creating-editing-overrides.md#edit-override-single-listing), and define the Refurbished condition for the listing.<br><br>**Note:** Not available for products set to `Fulfilled by Amazon`. |
|Seller Notes|An override that defines the _Seller Notes_ section of the listing. This field can be used to add additional information related to the product or the override applied, typically used to describe the condition of "non-new" products. Text in this field appears with the listing for the shopper. Seller notes cannot be added for a listing with a condition value of `New`. <br><br>**Example**: You have a product that is in `Refurbished` condition. Normally products in this condition do not include any manuals or documents, but you have a different supplier for this product that includes a manual. You can view the listing, [create a seller notes override](./creating-editing-overrides.md#edit-override-single-listing), and add your text note that is unique to this listing about the manual so the shopper knows it is included.<br><br>**Note**: If a product has a defined condition of `New`, you can enter a seller notes override, but Amazon does not display seller notes for a `New` product.|

You can create, edit, or remove an override for a [single listing](./creating-editing-overrides.md#edit-override-single-listing). On the _[!UICONTROL Inactive]_, _[!UICONTROL Active]_, and _[!UICONTROL Ineligible]_ tabs, you can click **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column and choose **[!UICONTROL Create Override]**. The _[!UICONTROL Edit Overrides]_ action is available only when a listing has an override applied and is viewed on the _[!UICONTROL Overrides]_ tab.

You can also create, edit, or remove an override to [multiple listings](./creating-editing-overrides.md#edit-override-multiple-listings). On the _[!UICONTROL Inactive]_, _[!UICONTROL Active]_, and _[!UICONTROL Ineligible]_ tabs, you can click **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column and choose **[!UICONTROL Edit Listing Overrides]**.

Removing an override tells the listing to use the values defined by your listing settings and rules.

When defining an override, you can also choose to enter a single type of override or any combination of the types.

See [Create and Edit Overrides](./creating-editing-overrides.md).

>[!NOTE]
>
>If you have listings in process, the number of listings is displayed in a message above the tabs.

![Overrides tab](assets/amazon-overrides.png)

Amazon sales channel home pages share some common [workspace controls](./workspace-controls.md) that allow you to customize the data that is displayed.

## Default columns

|Column|Description|
|---|---|
|[!UICONTROL Amazon Seller SKU]|The SKU (Stock Keeping Unit) assigned by Amazon to a product to identify the product, options, price, and manufacturer. |
|[!UICONTROL ASIN]|A unique block of 10 letters and/or numbers that identify items.<br><br>ASIN stands for the Amazon Standard Identification Numbers. An ASIN is a unique block of 10 letters and/or numbers that identify items. For books, the ASIN is the same as the ISBN number, but for all other products a new ASIN is created when the item is uploaded to their catalog. You can find an items ASIN on the product detail page on Amazon, along with further details relating to the item. |
|[!UICONTROL Condition Override]|The new condition defined in the override. If the override applied to the listing is not a condition override, `Not Selected` appears in this column. |
|[!UICONTROL Product Listing Name]|The name of the product. |
|[!UICONTROL Seller Notes Override]|The new seller notes defined in the override. If the override applied to the listing is not this type of override, this column is blank. |
|[!UICONTROL Handling Override]|The new handling time defined in the override (in days). If the override applied to the listing is not a handling time override, this column is blank. |
|[!UICONTROL List Price Override]|The new listing price defined in the override. If the override applied to the listing is not a price override, `N/A` appears in this column. |
|[!UICONTROL Action]|List of available actions that can be applied to a specific listing. To apply an action, in the _[!UICONTROL Action]_ column, click **[!UICONTROL Select]** and choose an option:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
