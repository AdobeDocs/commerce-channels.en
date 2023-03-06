---
title: 'Intelligent Repricing Rule: Optional Ceiling Price'
description: Use optional ceiling price settings to protect your highest product price against the intelligent pricing rules that manage your Amazon listings.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
---
# Intelligent Repricing Rule: Optional Ceiling Price

Sections of an intelligent repricing rule include:

- [Select Rule Type](./intelligent-repricing-rules.md)
- [Competitor Conditional Variances](./competitor-conditional-variances.md)
- [Price Adjustment](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- Optional Ceiling Price

The automated ceiling price settings automatically protect your highest product price against the intelligent pricing rules, enabling you to set a ceiling (highest price) for your intelligent pricing rules.

## Configure optional ceiling price

Define your optional highest price settings in the _[!UICONTROL Optional Ceiling Price]_ section.

1. For **[!UICONTROL Ceiling Price Source]**, choose an attribute.

   Select your [!DNL Commerce] [product attribute](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} that indicates your relative ceiling limit. For example, if you do not want your Amazon listing price to go above the MSRP of your item, you would choose the `Manufacturer's Suggested Retail Price` attribute.

1. For **[!UICONTROL Ceiling Price Action]**, choose an option.

   - `Decrease By` - Choose when you want the defined _[!UICONTROL Ceiling Price Source]_ value to be adjusted down, creating a lower ceiling price for the rule, before listing to Amazon.

   - `Increase By` - Choose when you want the defined _[!UICONTROL Ceiling Price Source]_ value to be adjusted up, creating a higher ceiling price for the rule, before listing to Amazon.

   - `Match` - Choose when you do not want the listing price to fluctuate above the defined _[!UICONTROL Ceiling Price Source]_ value. When set to `Match`, the _[!UICONTROL Apply]_ and _[!UICONTROL Ceiling Adjustment Amount]_ fields are disabled.

1. Leave the **[!UICONTROL Apply]** default as `Apply as percentage`.

1. For **[!UICONTROL Ceiling Adjustment Price]**, enter the numerical value for the percent to adjust your _[!UICONTROL Ceiling Price Source]_ value.

In this example, the ceiling price is set to be 2% below the MSRP of the item.

![Intelligent repricing rule - optional ceiling price](assets/ob-intelligent-price-rule-ceiling.png)

|Field |Description|
|---|---|
|[!UICONTROL Ceiling Price Source]|Choose the [!DNL Commerce] [product attribute](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} that indicates your relative ceiling limit. For example, if you do not want your product listing price to go above the MSRP of your item, you would choose the `Manufacturer's Suggested Retail Price` attribute. |
|[!UICONTROL Ceiling Price Action] |Choose a pricing adjustment action. Options:<ul><li>**[!UICONTROL Decrease By]** - Choose when you want the defined _[!UICONTROL Ceiling Price Source]_ value to be adjusted down, creating a lower ceiling price for the rule, before listing to Amazon.</li><li>**[!UICONTROL Increase By]** - Choose when you want the defined _[!UICONTROL Ceiling Price Source]_ value to be adjusted up, creating a higher ceiling price for the rule, before listing to Amazon.</li><li>**[!UICONTROL Match]** - Choose when you do not want the listing price to fluctuate above the defined _[!UICONTROL Ceiling Price Source]_ value. When set to `Match`, the _[!UICONTROL Apply]_ and _[!UICONTROL Ceiling Adjustment Amount]_ fields are disabled.</li></ul> |
|[!UICONTROL Apply]|**[!UICONTROL Apply as percentage]** - A percentage adjustment relative to the _[!UICONTROL Ceiling Price Source]_ value. |
|[!UICONTROL Ceiling Price Adjustment]|Enter the numerical value for the percent to adjust your _[!UICONTROL Ceiling Price Source]_ value. |
