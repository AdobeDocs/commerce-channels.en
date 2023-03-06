---
title: Create and Assign Products
description: Amazon Sales Channel provides the [!UICONTROL New Third Party] tab to help create and assign matching Commerce catalog products with Amazon listings.
exl-id: de000e80-7546-44d2-905e-28664b24f028
---
# Create and Assign Products

When viewing _[!UICONTROL New Third Party]_ tab, you can match your [!DNL Commerce] catalog products to an existing Amazon listing. There are two options for this matching. You can assign a listing to an existing catalog product, or you can use the information from the listing to create catalog products. These options are helpful when your Amazon listings do not automatically match to your [!DNL Commerce] catalog.

Matching (or assigning) your products to your Amazon listings is necessary to use the full feature set of Amazon sales channel.

When you create a catalog product from an Amazon listing:

- The **ASIN** becomes the [!DNL Commerce] SKU
- The **Product Listing Name** becomes the Catalog Listing Name
- The **Price** and **Quantity** are imported from the Amazon Listing

The rest of the necessary settings are determined by the [!DNL Commerce] product settings you select during creation.

When created and matched, the listings remove from the _[!UICONTROL New Third Party]_ tab and appear on the _[!UICONTROL Active]_ tab.

## Assign a single catalog product to an Amazon listing

1. View your product listings on the [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) tab.

1. Find the listing you wish to assign in the list, click **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column, and click **[!UICONTROL Assign Catalog Product]**.

   This action opens the _[!UICONTROL Assign Magento Catalog Product]_ page.

1. Browse for or filter the list using the [workspace controls](./workspace-controls.md) and locate the appropriate catalog product to match to the listing.

1. When the correct product appears in the list, click **[!UICONTROL Assign Catalog Product]** in the _[!UICONTROL Action]_ column.

Your product and listing are now matched. Amazon sales channel can now share product and listing data with Amazon and manage your listing and its information, including listing price, shipping price, stock/quantity, order information and status, and more.

## Create a single catalog product using the Amazon listing information

1. View your product listings on the [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) tab.

1. Find the listing you wish to create in your [!DNL Commerce] catalog, click **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column, and click **[!UICONTROL Create New Catalog Product]**.

   This action opens the _[!UICONTROL Create Magento Catalog Product]_ page.

1. Complete the catalog settings for the product.

   - Set **[!UICONTROL Enable Product(s)]** toggle to `Yes` or `No` (required).

      |Yes|Choose to make the product eligible for your [!DNL Commerce] storefront sales.|
      |No|Choose to make the product ineligible for your [!DNL Commerce] storefront sales.|

   - For **[!UICONTROL Categories]**, assign a category for the product (optional).

      To select the product's category, click the down arrow and select a category checkbox. Click **[!UICONTROL Done]** when finished.

   - For **[!UICONTROL Website Ids]**, choose the website (storefront) for which the product to be associated.

      The options in this list depend on your [!DNL Commerce] [store configuration](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} settings.

   - For **[!UICONTROL Attribute Set Id]** (required), choose an option.

      `Default` is the default selection. The options in this list depend on your [!DNL Commerce] [attribute sets](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} you have configured.

   - For **[!UICONTROL Visibility]**, choose an option for the new product.

      |**[!UICONTROL Not Visible Individually]** (default)|The product is not included in your storefront listings, although it might be available as a variation of another product.|
      |**[!UICONTROL Catalog]**|The product appears in your catalog listings.|
      |**[!UICONTROL Search]**|The product is available for search operations.|
      |**[!UICONTROL Catalog and Search]**|The product is included in catalog listings and available for search operations.|

   - For **[!UICONTROL Assign Tax Class]**, choose an option for the product.

      The options that display in this list depend on the [tax classes](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} you have configured.

   - When complete, click **[!UICONTROL Create Catalog Products]**.

The catalog product is created in your [!DNL Commerce] catalog and assigned to the Amazon listing from which it was created. With the listing now matched to an existing Amazon listing, the listing is removed from the _[!UICONTROL New Third Party]_ tab and appear in the _[!UICONTROL Active]_ tab.

## Create multiple catalog products using their Amazon listing information

1. View your product listings on the [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) tab.

1. Select the listings for which to create catalog products.

   You can select individual checkboxes in the left-side column, or you can click the down arrow in the top-left column and choose **[!UICONTROL Select All]** or **[!UICONTROL Select All on this Page]**.

1. Under _[!UICONTROL Actions]_, click **[!UICONTROL Create New Catalog Product(s)]**.

1. To accept the confirmation message and open the _[!UICONTROL Create Magento Catalog Product]_ page, click **[!UICONTROL OK]**.

1. Complete the catalog settings for the products.

   >[!NOTE]
   >When creating catalog products for multiple selected listings, the product settings entered are applied to all the listings.

   - Set **[!UICONTROL Enable Product(s)]** toggle to `Yes` or `No` (required).

      |Yes|Choose to make the product eligible for your [!DNL Commerce] storefront sales.|
      |No|Choose to make the product ineligible for your [!DNL Commerce] storefront sales.|

   - For **[!UICONTROL Categories]**, assign a category for the product (optional).

      To select the product's category, click the down arrow and select a category checkbox. Click **Done** when finished.

   - For **[!UICONTROL Website Ids]**, choose the website (storefront) for which the product to be associated.

      The options in this list depend on your [!DNL Commerce] [store configuration](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} settings.

   - For **[!UICONTROL Attribute Set Id]** (required), choose an option.

      `Default` is the default selection. The options in this list depend on your [!DNL Commerce] [attribute sets](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"} you have configured.

   - For **[!UICONTROL Visibility]**, choose an option for the new product.

      |**[!UICONTROL Not Visible Individually]** (default)|The product is not included in your storefront listings, although it might be available as a variation of another product.|
      |**[!UICONTROL Catalog]**|The product appears in your catalog listings.|
      |**[!UICONTROL Search]**|The product is available for search operations.|
      |**[!UICONTROL Catalog and Search]**|The product is included in catalog listings and available for search operations.|

   - For **[!UICONTROL Assign Tax Class]**, choose an option for the product.

      The options that display in this list depend on the [tax classes](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"} you have configured.

   - When complete, click **[!UICONTROL Create Catalog Products]**.

The catalog products are created in your [!DNL Commerce] catalog and assigned to the Amazon listing from which it was created. With the listings now matched to their respective Amazon listing, the listings are removed from the [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) tab and appear in the [_[!UICONTROL Active]_](./active-listings.md) tab.

![Create Commerce catalog product](assets/amazon-magento-catalog-product.png)

|Field|Description|
|--- |--- |
|[!UICONTROL Enable Product(s)]|(Required) If enabled, the product is visible in your [!DNL Commerce] storefront. If disabled, the product does not show in your [!DNL Commerce] storefront.|
|[!UICONTROL Categories]|You can enter the name of the category for your new product or select a category by clicking the down arrow to show your options. Options depend on your [categories](https://docs.magento.com/user-guide/catalog/category-create.html){target="_blank"} configuration.|
|[!UICONTROL Website Ids]|(Required) Choose the website (storefront) for which the product to be associated. Options depend on your [!DNL Commerce] [store configuration](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} settings|
|Attribute Set Id|Choose an attribute set. Options depend on your configured [!DNL Commerce] [attribute sets](https://docs.magento.com/user-guide/stores/attribute-sets.html){target="_blank"}.|
|[!UICONTROL Visibility]|Options:<ul><li>**[!UICONTROL Not Visible Individually]** - The product is not visible in your [!DNL Commerce] storefront (most common for variant products).</li><li>**[!UICONTROL Catalog]** - Allows the product to be accessed through the category it is associated to within the website.</li><li>**Search** - Allows the product to only be found through the search tool.</li><li>**[!UICONTROL Catalog and Search]** - Allows the products to be accessed through the category structure and by using the search tool.</li></ul> |
|[!UICONTROL Assign Tax Class]|Assign a tax class to the new product. Options depend on your configured [tax classes](https://docs.magento.com/user-guide/tax/tax-class.html){target="_blank"}.|
