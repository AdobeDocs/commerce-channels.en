---
title: Create an Alias Amazon Seller SKU
description: You can use the Alias Amazon Seller SKU to create multi-regional Amazon listings from your Commerce catalog products.
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
---
# Create an Alias Amazon Seller SKU

An [!DNL Alias Amazon Seller SKU] is used to create an Amazon listing from same product in your [!DNL Commerce] catalog. If you are an experienced Amazon seller, you may be familiar with the [Amazon Global SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target="_blank"} and Marketplace-specific SKU for inventory and shipping. Following similar principles for Amazon sales channel, the Amazon Seller SKU controls product listing information at multi-regional level, and the [!DNL Alias Amazon Seller SKU] can be used to control product listing information at a region-specific level.

This function can be used to perform two functions:

- Create an [!DNL Alias Amazon Seller SKU] for one of your [!DNL Commerce] catalog products to control region-specific listing information.

    **Example**: You are a seller in both the US and the Canada regions. Remember, each of your Amazon sales channel stores can only be assigned one Amazon region during setup. So, you have an Amazon sales channel store with a defined US region and another store with a defined Canada region. Both stores share your [!DNL Commerce] catalog for listing information across both regions, including the Amazon Seller SKU and ASIN product attributes. So, listings for the catalog product would be the same in both stores, sharing pricing, stock/quantity, and other product attributes. But, your stock for your Canada store ships from a Canada location, and your US store ships from a US location. Thus, you should control the listing quantity for the listing separately for each store. To accomplish this type of region-specific control, you can create an Alias Amazon Seller SKU.

    Essentially, you can create an Alias Amazon Seller SKU that is linked to the same catalog product and can be used to republish the same listing in that region.

- Create an [!DNL Alias Amazon Seller SKU] and match one of your [!DNL Commerce] catalog products to two Amazon listings.

    **Example**: You have a catalog product that is matched to an Amazon listing. As Amazon frequently has multiple listings that represent the same product, you discover another Amazon listing for the same product, but Amazon has assigned a different ASIN to the listing. To increase your product visibility to include, you want to match your catalog product to the different ASIN and create listings for both ASIN values. To accomplish this, you can create an Alias Amazon Seller SKU.

    Essentially, you can create an [!DNL Alias Amazon Seller SKU] that can be used to match a single catalog product to a second Amazon listing and create a listing for the newly matched ASIN. In this scenario, you would have two Amazon listings for the same catalog product.

    After you've created an Alias Amazon Seller SKU, you can use your listing settings, rules, and overrides to control the listing information for the region. Product attributes that can be defined per region for a listing include quantity/stock, fulfillment method, condition, product eligibility, and handling time.

## Used for a region-specific purpose {#region-specific}

View the listing on the _[!UICONTROL Product Listings]_ page (_[!UICONTROL Inactive]_, _Active_, _Ineligible_, or _Ended_ tab).

1. Under _[!UICONTROL Actions]_, click **[!UICONTROL Create Alias Seller SKU]**.

1. For **[!UICONTROL Assign New Seller SKU]**, enter a unique alphanumeric value.

    This value must be unique (not used for any other product or alias in your catalog).

1. For **[!UICONTROL Assign New ASIN]**, make no change.

    This value auto-populates with the product ASIN that is matched to your catalog product. Changing this value matches your catalog product to two Amazon listings based on the ASIN.

1. Toggle the **[!UICONTROL Remove Existing Seller SKU]** option as needed.

   - `Yes` - Choose to delete the listing and create a listing using the new information provided.

   - `No` - Choose to create a listing and keep the old listing unchanged.

1. Click **[!UICONTROL Save Listing Update]**.

## Used to match a single catalog product to two Amazon listings

1. View the listing on the _[!UICONTROL Product Listings]_ page (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, _[!UICONTROL Ineligible]_, or _[!UICONTROL Ended]_ tabs).

1. Under _[!UICONTROL Actions]_, click **[!UICONTROL Create Alias Seller SKU]**.

1. For **[!UICONTROL Assign New Seller SKU]**, enter a unique alphanumeric value.

    This value must be unique (not used for any other product or alias in your catalog).

1. For **[!UICONTROL Assign New ASIN]**, enter a unique alphanumeric value.

    This value auto-populates with the product ASIN that is matched to your catalog product. Changing this value matches your catalog product to two Amazon listings based on the ASIN.

1. Toggle the **[!UICONTROL Remove Existing Seller SKU]** option as needed.

   - `Yes` - Choose to delete the listing and create a listing using the new information provided.

   - `No` - Choose to create another listing and keep the old listing unchanged.

1. Click **[!UICONTROL Save Listing Update]**.

![create an Alias Amazon Seller SKU](assets/amazon-alias-sku-create.png){width="600" zoomable="yes"}

|Field|Description|
|--- |--- |
|[!UICONTROL Assign New Seller SKU]|Enter a new, unique alphanumeric value to be linked to the original Amazon Seller SKU. This number is only used by Amazon sales channel to match to your catalog product. You can use any SKU value, but the value can only be used once in your catalog. |
|[!UICONTROL Assign New ASIN]|Enter the ASIN value for the listing to which you want to match your catalog product. Only modify this field when matching a single catalog product to the ASIN for another listing for the same product. This value must match the ASIN assigned by Amazon or the listing will not be rejected by Amazon. |
|[!UICONTROL Remove Existing Seller SKU]|Options:<ul><li>**[!UICONTROL Yes]** - Choose to delete the listing and create a listing using the new information provided. The new listing appears in the _[!UICONTROL Active]_ tab, and the old listing moves to the _Ended_ tab.</li><li>**[!UICONTROL No]** - Choose to create another listing and keep the old listing unchanged. Both listings appear in the Active tab after the new listing is created.</li></ul> |
