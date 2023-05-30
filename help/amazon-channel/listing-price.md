---
title: Listing Price
description: Use the Listing Price settings to determine price source and the base (default) price value for your Amazon listings.
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
---
# Listing Price

[!UICONTROL Listing Price] settings are part of your store listing settings. Listing settings are accessed from the [store dashboard](./amazon-store-dashboard.md).

These settings define which [!DNL Commerce] pricing attribute to use as your price source, which is the base (default) price value for your Amazon listings. These settings are used by your [pricing rules](./pricing-rule-general-settings.md) to automatically adjust your Amazon listing price relative to the value set for _[!UICONTROL Magento Price Source]_.

You can configure your [pricing scope](./price-scope.md) as global or website. If your pricing scope is set to `Global`, there is a single price source for all your stores/websites. If your pricing scope is set to `Website`, the price source uses fallback logic of website price (if available) followed by the default (global) price.

If a listing rule is set to apply to more than one website, the order in which website price is used is determined by the website priority setting defined in the [listing rule](./listing-rules.md). These rules allow you to define product pricing across your catalog. To see if you are using website price scope, see [Catalog Price Scope](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html).

The options listed in _[!UICONTROL Magento Price Source]_, _[!UICONTROL Minimum Advertised Price (Map)]_, and _[!UICONTROL Strike Through Price (MSRP)]_ include your configured Pricing attributes. Pricing attributes are [!DNL Commerce] product attributes with the Catalog Input Type for Store Owner value set to `Price`. See [Attribute Input Types](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/attributes-input-types.html).

## Configure Listing Price settings {#configure-listing-price-settings}

1. Click **[!UICONTROL Listing Settings]** on the store dashboard.

1. Expand the _[!UICONTROL Listing Price]_ section.

1. For **[!UICONTROL Magento Price Source]** (required), choose an option.

   The default is `Price`. This setting determines the price source used for your Amazon listings. If you create [pricing rules](./pricing-products.md), the rules are applied to the value defined for the attribute selected here. You can select any configured pricing attribute. However, if the selected attribute is not filled in for a product, the price source for the product defaults back to `Price` when pricing rules are applied to determine the published Amazon listing price.

1. For **[!UICONTROL Minimum Advertised Price (MAP)**], choose an option.

   The default is no selection. This setting enables a minimum advertised price (MAP) for a product. When you define a pricing attribute and your listing price for a product falls below your determined minimum price (based on your pricing source and rules), this value becomes the MAP for the listing. This setting allows you to implement [pricing rules](./pricing-products.md), while still controlling your minimum price for a product. To prevent a listing price from being too low, choose a pricing attribute to use as your MAP. However, if the selected pricing field is not defined for a product, the MAP is not used.

1. For **[!UICONTROL Strike Through Price (MSRP)]**, choose an option.

   The default is no selection. This setting determines which pricing attribute is used as the manufacturer's suggested retail price (MSRP) for a product. If your listing price is less than the defined MSRP, your Amazon listing is displayed with a strike-through of the MSRP price with the lower listing price, along with the calculated "You Save" amount and percentage. However, if the selected pricing field is not defined for a product, the MSRP is not calculated.

   >[!NOTE]
   >
   >This setting only applies to listings that have won the [Buy Box](./buy-box-competitor-pricing.md) position. The Buy Box is awarded by Amazon to the seller who has the product listed usually at the best price, along with other factors such as FBA/Prime shipping offered, availability, and the seller's performance.

1. For **Apply Value Added Tax (VAT)**, choose an option:

   - `Disabled` - (Default) Choose when you do not want to apply VAT to your listing price.

   - `Enabled` - Choose when you want to apply VAT to your listing price. VAT is typically used as a sales tax in European countries and is added to your final listed price within Amazon. VAT does not apply to final price for listings that are used within an intelligent pricing rule, unless the [floor price](./floor-price.md) is hit.

   >[!NOTE]
   >
   >Businesses in the European Union (EU) are required to send invoices to business buyers, so that the customer can remit tax. You can either generate these invoices and calculate the taxes yourself or use a tax calculation service such as Amazon's VAT Calculation Service. Amazon recommends signing up for the [Amazon VAT Calculation Service](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&). If you choose a different method, you are responsible for VAT compliance.>
   >
   >It may take 10-14 days for Amazon to verify and activate your VAT Calculation Service account.

1. For **[!UICONTROL VAT Percentage]**, enter the value for your VAT rate.

   The default is `0.00`. This value is used to calculate the VAT amount to be added to the listing price. If `10.2` is entered, a 10.20% VAT is applied to your listing price. This field is disabled when the Apply Value Added Tax (VAT) field is set to `Disabled`.

1. **(UK Stores Only)** For **[!UICONTROL Amazon Product Tax Code (PTC)]**, choose an option:

   - `Do Not Manage PTC` - (Default) Choose if you are using a third-party tax calculation service or already have all your tax calculations set up in your [!DNL Amazon Seller Central] account. When chosen, Amazon sales channel sends no product tax code information to your [!DNL Amazon Seller Central] account.

   - `Set Default PTC` - Choose if you have a universal product tax code (PTC) you want to use for all your products. When chosen, you must complete _[!UICONTROL Default PTC]_.

      - For **[!UICONTROL Default PTC]**, enter the default PTC to be used for all eligible Amazon listings. If your default PTC is set in your [!DNL Amazon Seller Central] account, leave this field blank. Changes made to this field do not affect existing Amazon listings. To change the Default PTC for an existing listing, the listing must be [ended](./end-listings-manually.md) and a new listing created.

   >[!NOTE]
   >
   >If you use Amazon's VAT Calculation Service, you must know the tax category for your products. A PTC is Amazon's tax category ID code for B2B purchases in the EU. See [Amazon's Product Tax Codes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&language=en_US){target="_blank"}.

1. For **[!UICONTROL Currency Conversion]**, choose an option.

   The default is `Disabled`. These options depend on your [!DNL Commerce] [currency](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) settings. If no options are available, set up your currency settings.

1. When complete, click **[!UICONTROL Save listing settings]**.

![Listing Price](assets/amazon-listing-price.png){width="500" zoomable="yes"}

|Field|Description|
|--- |--- |
|[!UICONTROL Magento Price Source] |Determines the price source that are used when creating your Amazon listings. The default is `Price`. If you choose a different attribute such as `Amazon Price` or `Special Price`, the defined value for the attribute is used for your Amazon listing. However, if selected attribute is not defined, `Price` is used. |
|[!UICONTROL Minimum Advertised Price (MAP)] |The [!DNL Commerce] attribute for MAP pricing. Choosing the MAP option automatically sets your Amazon listing to the MAP price if the listing price is less than the MAP price. |
|[!UICONTROL Strike Through Price (MSRP)] |The [!DNL Commerce] attribute that represents the MSRP pricing. If your Amazon listing price is less than the MSRP, it displays a strike-through of the MSRP price and the listing price. This setting is also used to calculate the "You Save" amount and percentage, but this feature only applies to listings that have won the [Buy Box](./buy-box-competitor-pricing.md) position. |
|[!UICONTROL Apply Value Added Tax (VAT)] |VAT is used by sellers in the European Union.<br><br>Choose `Disabled` if you do not want VAT added to listing prices.<br><br>Choose `Enabled` and then enter the VAT Percentage for applying VAT to your listing prices.|
|[!UICONTROL VAT Percentage]|Define the percentage to be used to calculate the VAT amount to be added to the listing price for your Amazon listings. <br><br>If you enter `5`, then a 5% VAT will be applied to the final listing price after all pricing rules have been applied. VAT tax does not apply to the final price for listings that are used within an intelligent pricing rule, unless the [floor](./floor-price.md) or [ceiling](./optional-ceiling-price.md) is hit. |
|[!UICONTROL Amazon Product Tax Code (PTC)]|(Appears for UK Stores Only) Determines if Amazon sales channel sends product tax code information to your [!DNL Amazon Seller Central] account. <br><br>Select **Do Not Manage PTC** if you are using a third-party tax calculation service or already have all your tax calculations set up in your [!DNL Amazon Seller Central] account. When set to this option, Amazon sales channel sends no product tax code information to your [!DNL Amazon Seller Central] account.<br><br>Select **Set Default PTC** if you have a universal product tax code you want to use for all your products.<br><br>See [Amazon's Product Tax Codes](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&language=en_US){target="_blank"}.|
|[!UICONTROL Default PTC]|Only appears when **Amazon Product Tax Code (PTC)** is set to `Set Default PTC`. Enter the default PTC to be used for all eligible Amazon listings. If your default PTC is set in your [!DNL Amazon Seller Central] account, leave this field blank. <br><br>Changes made to this field do not affect existing listings. The listing must be [ended](./end-listings-manually.md) and a new listing created for the change to take effect.|
|[!UICONTROL Currency Conversion] |Allows your [!DNL Commerce] storefront default currency to accurately convert to your default Amazon currency to publish your listing prices in the proper currency. The currency conversion is always based on your [!DNL Commerce] default currency.<br><br>You can still view your default [!DNL Commerce] and Amazon currencies when other currencies are available. If your default [!DNL Commerce] currency matches your default Amazon currency, leave Currency Conversion disabled.<br><br>For example, if your [!DNL Commerce] default currency is CAD (Canadian Dollars) and your Amazon default currency is USD, you must enable Currency Conversion and choose the Conversion Rate CAD to USD. The options presented are based on the built-in [!DNL Commerce] currency conversions. If you do not see the option that you are looking for, [set up the currency in [!DNL Commerce]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html). |

**Quick Access** - [!UICONTROL Listing Settings] sections

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
