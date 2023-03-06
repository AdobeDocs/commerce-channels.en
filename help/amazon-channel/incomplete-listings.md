---
title: Incomplete Listings
description: Amazon sales channel provides the [!UICONTROL Incomplete] tab to help you identify and meet eligibility requirements for your incomplete Amazon listings.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
---
# Incomplete Listings

The _[!UICONTROL Incomplete]_ tab lists the [!DNL Commerce] catalog products that meet your Amazon eligibility requirements (defined in your [listing rules](./listing-rules.md)), but are missing information required by Amazon (such as the Amazon ASIN or a defined product condition).

There are four possible causes for an incomplete listing, each identified by its status.

|Status|Reason|Action|
|--- |--- |--- |
|Missing Condition|Amazon accepts listings in various conditions (such as _New_, _Refurbished_, _Used: Like New_) listing requires a defined condition.|Update required info and manually [assign a condition](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) to a listing.|
|Unable to Assign to Amazon Listing|Automatic match of this listing to your catalog failed. If no match is found, the listing cannot be managed by Amazon Sales Channel|Update required info and manually [assign an ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) to the catalog product for matching to the listing.|
|Multiple Matches Found|Automatic match of this listing to your catalog failed. If multiple possible matches are found, you must select the correct match for your product.|Update required info and manually [choose a product match](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) for the product and listing.|
|Has Variants|If your product has variants, such as a t-shirt that is available in different sizes or colors, you must choose the variant in your catalog to be correctly assigned and matched to the listing|Update required info and manually [choose the correct variant](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) to assign and match to this listing.|

>[!NOTE]
>When incomplete listings are properly matched to your catalog products, the listing moves from the _[!UICONTROL Incomplete]_ tab and are published to Amazon based on your [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) settings.

The available actions on the _[!UICONTROL Incomplete]_ tab include:

Under _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Choose to initiate the automatic process for matching your Amazon listings data to your [!DNL Commerce] catalog. If products are not automatically matching, revisit your [_[!UICONTROL Catalog Search]_](./catalog-search.md) options in your listing lettings. If listings do not automatically match after updating your _[!UICONTROL Catalog Search]_ options, you can match products manually in the [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) action.

Under **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column:

- **[!UICONTROL Update Required Info]**: Choose when listings do not automatically match to your catalog. You can manually [match catalog products to listings](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), manually [assign an ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) to a catalog match, or [assign a missing condition](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) for listing.

- **[!UICONTROL View Details]**: Choose to view listing details, including the [Listing Activity Log](./product-listing-details.md#listing-activity-log), [Buy Box Competitor Pricing](./product-listing-details.md#buy-box-competitor-pricing), and [Lowest Competitor Pricing](./product-listing-details.md#lowest-competitor-pricing). This action is for viewing only. No changes can be made in the listing details. See [View Details](./product-listing-details.md).

>[!NOTE]
>
>If you have listings in process, the number of listings appears in a message above the tabs.

![Incomplete Amazon listings](assets/amazon-incomplete-listings.png)

Amazon sales channel home pages share some common [workspace controls](./workspace-controls.md) that allow you to customize the data that is displayed.

|Column|Description|
|--- |--- |
|[!UICONTROL Amazon Seller SKU]|The SKU (Stock Keeping Unit) assigned by Amazon to a product to identify the product, options, price, and manufacturer.|
|[!UICONTROL ASIN]|A unique block of 10 letters and/or numbers that identify items.<br><br>ASIN stands for the [!DNL Amazon Standard Identification Number]. An ASIN is a unique block of 10 letters and/or numbers that identify items. For books, the ASIN is the same as the ISBN number, but for all other products a new ASIN is created when the item is uploaded to their catalog. You can find an items ASIN on the product detail page on Amazon, along with further details relating to the item.|
|[!UICONTROL Product Listing Name]|The name of the product.|
|[!UICONTROL Condition]|The [condition](./product-listing-condition.md) of the product.|
|[!UICONTROL Landed Price]|The listing price for the product plus its shipping price.|
|[!UICONTROL Amazon Quantity]|The quantity available when the product is actively listed on Amazon.|
|[!UICONTROL Status]|The status of the listing, defined by Amazon. See the Status table above.|
|[!UICONTROL Action]|List of available actions that can be applied to a specific listing. To apply an action, click **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column and select an option:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul>|
