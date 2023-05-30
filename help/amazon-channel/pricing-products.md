---
title: Manage Amazon pricing
description: You can set pricing for your Amazon listings to differ from your COmmerce store by using the pricing rules.
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
---
# Manage Amazon pricing

Amazon sales channel allows you to set pricing rules, which allow you to set your Amazon listing price different from the defined **[!UICONTROL Magento Price Source]** in your [listing price](./listing-price.md). You can also stack multiple rules and even use the intelligent pricing to adjust your Amazon listing price based on competitors' [[!DNL Buy Box]](./buy-box-competitor-pricing.md) price or the [lowest competitor price](./lowest-competitor-pricing.md).

There are two types of pricing rules:

- [Standard Pricing Rule](./standard-price-rules.md)
- [Intelligent Repricing Rule](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Intelligent repricing rules do not function properly if the Amazon region is set to `Inactive` status, as it is during onboarding. Your pricing calculations depend on your shipping rates, and your region must be in `Active` status for your shipping rates to sync from Amazon.
   >
   >To update your region status in your Amazon account, go to Settings > Account Info > Vacation Settings. Refer to [Amazon: Listing Status for Vacations](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620) (Seller Central login required).

This feature allows you to manipulate your Amazon prices in a way that is similar to the [!DNL Commerce] [catalog price rules](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html). You can create complex rules that allow you to change prices for specific products, products inside specific categories, or even with specific attributes.

You can add pricing rules for your Amazon listings. Price rules can be used to automatically adjust your listing prices, based on a set of defined conditions. Price rules are triggered and calculate your adjusted price before your product is listed on Amazon.

>[!NOTE]
>
>The price source for your Amazon listings is defined for **[!UICONTROL Magento Price Source]** in your [listing price](./listing-price.md) settings. Any adjustment calculations defined in the pricing rule use price source as the starting value.

Pricing rules allow you to set your Amazon listing price different from your **[!UICONTROL Magento Price Source]** in your [listing price](./listing-price.md) settings. You can also stack multiple rules that work together to adjust your price.

A pricing/repricing rule requires three sets of information during its setup:

- [General settings](./pricing-rule-general-settings.md): Defines the name, description, active dates, priority for a rule and sets the behavior of subsequent rules, based on its priority setting.
- [Conditions](./pricing-rule-conditions.md): Determine which products are eligible for the price rule.
- [Actions](./pricing-rule-actions.md): Define the adjustment calculations that are applied to the price source to determine the listing price.

You can create [standard pricing rules](./standard-price-rules.md) that automatically adjust your Amazon listing price relative to the selected **[!UICONTROL Magento Price Source]** in your [listing price](./listing-price.md) settings. This feature allows you to manipulate your Amazon prices in a way that is similar to the [!DNL Commerce] [catalog price rules](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html). You can create complex rules that automatically change prices for specific products, products inside specific categories, or products with specific attributes. You can complete traditional settings and reprice your products to increase or decrease based on a fixed amount or a percentage.

Another powerful tool is the [Intelligent Repricing](./intelligent-repricing-rules.md) feature that adjusts your Amazon listing price based on competitor [[!DNL Buy Box]](./buy-box-competitor-pricing.md) price or [Lowest Competitor Price](./lowest-competitor-pricing.md). Similar to the [!DNL Commerce] [catalog price rules](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html), this advanced feature allows you to manipulate your Amazon prices by creating complex rules. Rules can define the scope for a price change for specific products, products inside specific categories, or even with specific product attributes.

Using intelligent repricing to adjust your Amazon listing prices, based on competitor's pricing. Amazon sales channel has built in safeguards for you to configure to protect margins or avoid matching the prices of a merchant with low feedback. Using [intelligent repricing rules](./intelligent-repricing-rules.md), Amazon listing prices can be automatically manipulated as a fixed or percentage amount (up or down) or even synchronized to the [[!DNL Buy Box]](./buy-box-competitor-pricing.md) price or [Lowest Competitor Price](./lowest-competitor-pricing.md) on a per item basis. Rules can even be stacked to provide unlimited flexibility.

You can control important aspects of rules, such as active/inactive status, website eligibility, optional date ranges, and optional priority levels (used for rule stacking).

For example, you can define and set the conditions for a price rule that, when the conditions are met, automatically adjust your listing price before it is sent to Amazon.

Another pricing option is a [price override](./overrides.md), which is set at the individual listing level. A [price override](./overrides.md) can be set, and an override ignores/takes priority over all other defaults, settings, and rules. An [override](./overrides.md) can be set for price, handling time, condition, and seller notes (with a few exceptions).

![Pricing rules](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## Default columns

|Column|Description|
|---|---|
|[!UICONTROL Name]|The name of the pricing rule, as set in [Pricing Rule General Settings](./pricing-rule-general-settings.md)|
|[!UICONTROL Rule Type]|The rule type, as set in [Pricing Rule Actions](./pricing-rule-actions.md) (either Standard price rule or Intelligent repricing rule)|
|[!UICONTROL Is Active]|Whether the rule is active, as set in [Pricing Rule General Settings](./pricing-rule-general-settings.md)|
|[!UICONTROL Priority]|The priority over other pricing conditions, as set in [Pricing Rule General Settings](./pricing-rule-general-settings.md)|
|[!UICONTROL Stop Further Rules Processing]|Indicates if any further price rules are processed on products eligible for this rule, as set in [pricing rule general settings](./pricing-rule-general-settings.md)|
|[!UICONTROL From Date]|The beginning of the time period in which the rule is active|
|[!UICONTROL To Date]|The end of the time period in which the rule is active|
|[!UICONTROL Action]|Lists all actions that can be applied to a specific listing. To apply an action, click **[!UICONTROL Select]** in the _[!UICONTROL Action]_ column. Options: `Edit Price Rule` / `Delete Price Rule`|
