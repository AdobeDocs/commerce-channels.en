---
title: Manage attributes for Amazon listings
description: You can manage the mapping of Commerce product attributes to the Amazon attributes to ensure accurate product information between the systems.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
---
# Manage attributes for Amazon listings

Amazon and [!DNL Commerce] both use a system of product properties, known as attributes, used to define a product. Attributes define the description, content, images, prices, and various data for your products.

Successful communication between Commerce and Amazon requires that [!DNL Commerce] attributes be correctly mapped (or matched) to the corresponding Amazon attribute. When integrating with Amazon, you map these attributes to Amazon attributes. When complete, [!DNL Commerce] can sync and maintain your Amazon listings with your [!DNL Commerce] product catalog.

For example, imagine you have the same item in your [!DNL Commerce] catalog and Amazon listings. One attribute for the product might be the listing price of the item. The name for the listing price in [!DNL Commerce] might be named `Price`, while the listing price for Amazon might be named `ListingPrice`. You must instruct [!DNL Commerce] that when communicating with Amazon, the [!DNL Commerce] attribute named `Price` is the same as the Amazon attribute named `ListingPrice`. This process is called _managing attributes_, and includes creating new and editing existing attributes. Making sure that attributes are properly matched ensures correct communication between [!DNL Commerce] and Amazon.

When attribute mapping is set up, [!DNL Commerce] can communicate product information back and forth with Amazon. If you have Amazon product listings, [!DNL Commerce] can import your Amazon products and details into your [!DNL Commerce] catalog, allowing you to manage your Amazon listings from a single, central catalog of products.

Amazon sales channel allows you to access, review, create, and manage attributes, as needed, in the [_[!UICONTROL Attributes]_ view](./attributes-view.md) on the Amazon sales channel home page. If you add an attribute to your [!DNL Commerce] catalog, it could require an update of those values across all products.

For more information about [!DNL Commerce] and Amazon attribute sets and values, see:

- [Manage attributes basics](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [Create an attribute](./creating-attributes.md#create-an-attribute)
- [Edit an existing attribute](./creating-attributes.md#edit-an-attribute)
- [View Attribute Mapping](./amazon-matching-attributes-values.md)
- [Edit or Create Attribute Mapping](./amazon-manually-update-incomplete-listing.md)
