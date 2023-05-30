---
title: Price Adjustment
description: Configure price adjustments to define the price calculation when you have identified the Amazon competitor price source.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
---
# Price Adjustment

>[!NOTE]
>
>The Price Adjustment section differs slightly for Standard and Intelligent repricing rules. **[!UICONTROL Match Competitor Price]** is only available under _[!UICONTROL Price Action]_ when **[!UICONTROL Rule Type]** is set to `Intelligent repricing rule`.

Sections of an intelligent repricing rule include:

- [Select Rule Type](./intelligent-repricing-rules.md)
- [Competitor Conditional Variances](./competitor-conditional-variances.md)
- Price Adjustment
- [Floor Price](./floor-price.md)
- [Optional Ceiling Price](./optional-ceiling-price.md)

The price adjustment defines the price calculation when you have identified the competitor price source.

## Configure price adjustment

Define your pricing adjustment in the _[!UICONTROL Price Adjustment]_ section.

1. For **[!UICONTROL Price Action]**, choose an option:

   - `Decrease By` - Choose when you want the defined price source value to be adjusted down, creating a lower price for the rule, before listing to Amazon.

   - `Increase By` - Choose when you want the defined price source value to be adjusted up, creating a higher price for the rule, before listing to Amazon.

   - `Match Competitor Price` - (Intelligent repricing rule only) Choose when you want to change your Amazon listing price to match the [lowest competitor](./lowest-competitor-pricing.md) price, based on your competitor feedback and variance parameters. When set to `Match Competitor Price`, the _[!UICONTROL Apply]_ and _[!UICONTROL Adjustment Amount]_ fields are removed.

1. For **[!UICONTROL Apply]**, choose an option:

   - `Apply as percentage` - Choose when you want the defined **[!UICONTROL Magento Price Source]** defined in your [Listing Price](./listing-price.md) adjusted by a percentage.

   - `Apply as fixed amount` - Choose when you want the defined **[!UICONTROL Magento Price Source]** defined in your [Listing Price](./listing-price.md) adjusted by a fixed amount.

1. For **[!UICONTROL Adjustment Amount]** (required), enter the numerical value for the price adjustment.

   - When **[!UICONTROL Apply]** is set to `Apply as percentage`, enter the percent value (example: enter `25` for a 25% percent adjustment).

   - When **[!UICONTROL Apply]** is set to `Apply as fixed amount`, enter the numerical value for the fixed amount (example: enter `25` for a $25 fixed adjustment).

![Intelligent repricing rule - price adjustment](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

|Field|Description|
|---|---|
|[!UICONTROL Price Action]|Choose a pricing adjustment action. Options:<br>**[!UICONTROL Decrease By]** - Choose when you want the defined _[!UICONTROL Magento Price Source]_ defined in your [Listing Price](./listing-price.md) to be adjusted down, creating a lower price for the rule, before listing to Amazon.<br>**[!UICONTROL Increase By]** - Choose when you want the defined _[!UICONTROL Magento Price Source]_ defined in your [Listing Price](./listing-price.md) to be adjusted up, creating a higher price for the rule, before listing to Amazon.<br>**[!UICONTROL Match Competitor Price]** - (Intelligent repricing rule only) Choose when you want to change your Amazon listing price to match the [lowest competitor](./lowest-competitor-pricing.md) price, based on your competitor feedback and variance parameters. When chosen, the _Apply_ and _Adjustment Amount_ fields are removed.|
|[!UICONTROL Apply]|Options:<br>**[!UICONTROL Apply as percentage]** - Choose when you want the defined _[!UICONTROL Magento Price Source]_ defined in your [Listing Price](./listing-price.md) adjusted by a percentage.<br>**[!UICONTROL Apply as fixed amount]** - Choose when you want the defined _[!UICONTROL Magento Price Source]_ defined in your [Listing Price](./listing-price.md) adjusted by a fixed amount.|
|[!UICONTROL Adjustment Amount]|Required.<br>If you chose `Apply as percentage` for **[!UICONTROL Apply]**, enter the percent value (example: enter `25` for a 25% percent adjustment).<br>If you chose `Apply as fixed amount` for **[!UICONTROL Apply]**, enter the  numerical value for the fixed amount (example: enter `25` for a $25 fixed adjustment).|
