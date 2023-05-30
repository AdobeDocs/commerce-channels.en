---
title: Create [!DNL Commerce] Attributes for Amazon
description: Before completing the Amazon sales channel onboarding process, make sure you have the needed [!UICONTROL Commerce] product attributes.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
---
# Create [!DNL Commerce] Attributes for Amazon

Before onboarding your [!DNL Amazon Seller Central] accounts, it is a best practice to add [!DNL Commerce] [product attributes](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) to map your product listings. After you complete onboarding, you can manage your product attributes through the [Attributes](./managing-attributes.md) tab of the [Amazon sales channel home](./amazon-sales-channel-home.md) page.

These instructions detail how to create [!DNL Commerce] attributes for Amazon ASIN and Amazon Condition. Creating additional attributes including Amazon EAN, Amazon ISBN, and Amazon UPC is recommended. You may want to also create an Amazon Price attribute if you want to use your Amazon listing price as a price source for pricing rules. These attributes are used when configuring your listing and pricing settings during onboarding. Also use these attributes when creating Amazon listings and when updating and syncing your [!DNL Commerce] catalog with your Amazon listings.

Catalog Search settings enable you to set matching search parameters that help to map eligible [!DNL Commerce] products with Amazon listings. When mapped, Amazon activates actions related to pricing, quantity, overrides, and order and product synchronization.

Defining these values increases the potential for exact matches, minimizing the need for manually matching product listings later. Adding the attributes as part of your onboarding [pre-setup tasks](./amazon-pre-setup-tasks.md), Amazon sales channel has a higher potential for automatically matching your products during onboarding and syncs product data between Amazon and [!DNL Commerce] after onboarding.

If you only create the Amazon ASIN attribute (without adding ASIN values per product), your [!DNL Commerce] products might not automatically match to your Amazon listings. You can manually match your products through _Store Review_. However, manual matching does not create the data elements that are required to share and sync your product data.

>[!IMPORTANT]
>
>If you update an ASIN, UPC, or other data element for a manually matched product, you must update the data in both places: your [!DNL Commerce] catalog and the listing in your [!DNL Amazon Seller Central] account.

## Create the Amazon ASIN product attribute

1. Log into your [!DNL Commerce] Admin.

1. Click **[!UICONTROL Stores]** in the left-side menu.

1. In the _[!UICONTROL Attributes]_ section, click **[!UICONTROL Product]**.

1. To open the attributes properties, click **[!UICONTROL Add New Attribute]**.

1. For **[!UICONTROL Default Label]**, enter `Amazon ASIN` (the name for your attribute).

1. For **[!UICONTROL Catalog Input Type for Store Owner]**, choose `Text Field`.

1. For **[!UICONTROL Values Required]**, choose `No`.

    Although an Amazon ASIN is required to list a product on Amazon, some of your catalog products may not be listed on Amazon.

1. Expand the _[!UICONTROL Advanced Attribute Properties]_ section and set the options:

   - For **[!UICONTROL Attribute Code]**, enter `amazon_asin`.

   - For **[!UICONTROL Scope]**, choose `Global`.

   - For **[!UICONTROL Unique Value]**, choose `No`.

   - For **[!UICONTROL Input Validation for Store Owner]**, choose `None`.

   - For **[!UICONTROL Add to Column Options]**, choose `Yes`.

   - For **[!UICONTROL Use in Filter Options]**, choose `Yes`.

1. Click **[!UICONTROL Save Attribute]**.

![Amazon ASIN attribute](assets/creating-asin-attribute.png){width="600" zoomable="yes"}

## Create the Amazon Condition product attribute

1. Log into your [!DNL Commerce] Admin.

1. Click **[!UICONTROL Stores]** in the left-side menu.

1. In the _[!UICONTROL Attributes]_ section, click **[!UICONTROL Product]**.

1. To open the attribute properties, click **[!UICONTROL Add New Attribute]**.

1. For **[!UICONTROL Default Label]**, enter `Amazon Condition` (the name for your attribute).

1. For **[!UICONTROL Catalog Input Type for Store Owner]**, choose `Dropdown`.

   The _[!UICONTROL Manage Options (Values of your Attribute)]_ section appears.

1. For **[!UICONTROL Values Required]**, choose `No`.

1. For **[!UICONTROL Manage Options (Values for your Attribute)]**, add each of your condition options.

   Standard Amazon conditions include:

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. Click **[!UICONTROL Add Option]**.

1. Select the **[!UICONTROL Is Default]** option for the condition you wish to be the default selection.

1. In the _[!UICONTROL Admin]_ column, enter the text for the label of the condition you are adding (such as `New`, `Used`, and `Used-Like New`)

1. Click **[!UICONTROL Add Option]** to add more options, as needed.

1. Expand _[!UICONTROL Advanced Attribute Properties]_ section and set the options.

   - For **[!UICONTROL Attribute Code]**, enter `amazon_condition`.

   - For **[!UICONTROL Scope]**, choose `Global`.

   - For **[!UICONTROL Unique Value]**, choose `No`.

   - For **[!UICONTROL Input Validation for Store Owner]**, choose `None`.

   - For **[!UICONTROL Add to Column Options]**, choose `Yes`.

   - For **[!UICONTROL Use in Filter Options]**, choose `Yes`.

1. Click **[!UICONTROL Save Attribute]**.

![Amazon Condition attribute](assets/creating-amazon-condition-attribute.png){width="600" zoomable="yes"}

![Next icon](assets/btn-next.png) [**Continue to Add or Verify API Key**](./amazon-verify-api-key.md)
