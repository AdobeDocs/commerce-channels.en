---
title: 'Intelligent Repricing Rule: Floor Price'
description: Use floor price settings to determine the lowest price for an intelligent pricing rule to manage your Amazon listings.
feature: Sales Channels, Price Rules
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
---
# Intelligent Repricing Rule: Floor Price

Sections of an intelligent repricing rule include:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

The [floor price](./floor-price.md) settings automatically protect your lowest product price against the intelligent pricing rules. Use these settings to set a floor (lowest price) for your intelligent pricing rules, ensuring that your products are not listed below a desired price.

Floor price attributes are based on the website scope if your [!DNL Commerce] store is using website pricing scope. See [Price Scope](./price-scope.md).

Floor price is only used when **[!UICONTROL Rule Type]** is set to `Intelligent repricing rule`.

## Configure floor price

Define your lowest price setting in the _[!UICONTROL Floor Price]_ section.

1. For **[!UICONTROL Floor Price Source]**, choose a price source attribute.

   Choose the [!DNL Commerce] [product attribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) that indicates your relative floor limit. For example, if you do not want your Amazon listing price to go below the cost of your item, you would choose the *Cost* attribute.

1. For **[!UICONTROL Floor Price Action]**, choose an option.

   - `Decrease By` - Choose when you want the defined _[!UICONTROL Floor Price Source]_ value to be adjusted down, creating a lower floor price for the rule, before listing to Amazon.

   - `Increase By` - Choose when you want the defined _[!UICONTROL Floor Price Source]_ value to be adjusted up, creating a higher floor price for the rule, before listing to Amazon.

   - `Match` - Choose when you do not want the listing price to fluctuate below the defined _[!UICONTROL Floor Price Source]_ value. When set to `Match`, the _[!UICONTROL Apply]_ and _[!UICONTROL Floor Adjustment Amount]_ fields are disabled.

1. Leave the **[!UICONTROL Apply]** default as `Apply as percentage`.

1. For **[!UICONTROL Floor Adjustment Price]**, enter the numerical value for the percent to adjust your _[!UICONTROL Floor Price Source]_ value.

In this example, the floor price is set to be 3% above the cost of the item.

![Intelligent repricing rule example - floor price](assets/ob-intelligent-pricde-rule-floor-price.png){width="600" zoomable="yes"}

| Field                                | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Floor Price Source]      | Choose the [!DNL Commerce] attribute that indicates your relative floor (lowest price) limit. For example, if you do not want your Amazon listing price to go below the cost of your item, you would choose the `Cost` attribute.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [!UICONTROL Floor Price Action]      | Choose a pricing adjustment action. Options:<ul><li>**[!UICONTROL Decrease By]** - Choose when you want the defined _[!UICONTROL Floor Price Source]_ value to be adjusted down, creating a lower floor price for the rule, before listing to Amazon.</li><li>**[!UICONTROL Increase By]** - Choose when you want the defined _[!UICONTROL Floor Price Source]_ value to be adjusted up, creating a higher floor price for the rule, before listing to Amazon.</li><li>**[!UICONTROL Match]** - Choose when you do not want the listing price to fluctuate below the defined _[!UICONTROL Floor Price Source]_ value. When chosen, the _[!UICONTROL Apply]_ and _[!UICONTROL Floor Adjustment Amount]_ fields are disabled.</li></ul> |
| [!UICONTROL Apply]                   | **[!UICONTROL Apply as percentage]** - A percentage adjustment relative to the _[!UICONTROL Floor Price Source]_ value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [!UICONTROL Floor Adjustment Amount] | Enter the numerical value for the percent to adjust your _[!UICONTROL Floor Price Source]_ value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
