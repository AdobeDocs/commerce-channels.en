---
title: Pricing Rule General Settings
description: Use the price rule general settings to define the primary characteristics of a listing price rule.
redirect_from: /sales-channels/asc/ob-pricing-rules-general-settings.html
exl-id: 915b3eed-997e-4f94-a23f-0553a9dfe30c
---
# Pricing Rule General Settings

Define the name, description, active dates, and priority for the rule.

## Complete the Price Rule General Settings section

1. For **[!UICONTROL Rule Name]** (required), enter the name for the rule.

   This name is for your internal identification purposes only. The more descriptive the rule name, the better.

1. For **[!UICONTROL Description]**, enter a detailed description of your rule.

   This description could include information on the products that qualify, the active dates, the formula for calculating your adjusted price, or any other information you'd find useful if you want to modify the rule.

1. For **[!UICONTROL Status]**, choose an option:

    - `Active` - Choose this option when you want the pricing rule to apply to your eligible products and adjust your listing pricing before publishing to Amazon.

    - `Inactive` - Choose this option when you do not want the pricing rule to apply to your eligible products. This option will most likely be used when modifying a pricing rule or turning it off after a limited promotion.

1. For **[!UICONTROL From]** and **[!UICONTROL To]**, enter a beginning and ending date for the pricing rule.

   You can also click the calendar icon to select a date from the dynamic calendar. This automatic start and stop option is beneficial when setting up limited-time or seasonal promotions with definite begin and end dates.

1. For **[!UICONTROL Priority]**, enter a numerical value for the rule priority.

   Priority value equal to `1` is the highest priority. When you have multiple active pricing rules, you can use this priority value to determine which rule is applied first. This field is required to use the _[!UICONTROL Discard Subsequent Rules]_ feature.

1. For **[!UICONTROL Discard Subsequent Rules]**, choose an option:

    - `Yes` - Choose this option when you do not want any other pricing rules that may apply to a product to be applied. Discarding subsequent rules means that, if multiple pricing rules apply to the same product, only the pricing rule with the highest defined priority value are applied to the product. This option prevents multiple pricing rules from stacking and providing unintended, additional discounts.

    - `No` - Choose this option when you want to allow multiple pricing rules to apply to the same product. This option could result in stacking and providing multiple discounts to be applied.

>[!NOTE]
>
>To discard subsequent rules, a pricing rule must have a define **Priority** value.

![Pricing rule general settings](assets/amazon-pricing-rule-general.png){width="600" zoomable="yes"}

|Field|Description|
|---|---|
|[!UICONTROL Rule Name]|(Required) Enter a name for the rule, used for internal identification purposes. The more descriptive the rule name, the better. For example, "25% off end of year book sale."|
|[!UICONTROL Description]|Enter a detailed description that explains the rule (also used for internal purposes). For example, "End of year sale, 25% off all items in the Books Category."|
|[!UICONTROL Status]|Options:<ul><li>**[!UICONTROL Inactive]** - The pricing rule does not apply to your listings. This option might be used when modifying a pricing rule or turning it off after a limited promotion.</li><li>**[!UICONTROL Active]** - The pricing rule applies to your listings and adjust your listing pricing before publishing to Amazon.</li></ul>|
|[!UICONTROL From]|Enter the start date when the pricing rule begins. For example, to have a sale during the last month of the year, you would set the `From` date to December 1 so that the pricing rule would automatically apply to your Amazon listings starting December 1.|
|[!UICONTROL To]|Enter the end date when the pricing rule ends. Continuing the previous example, to limit the sale to the last month of the year, you would set the `To` date as December 31, so the pricing rule expires on December 31.|
|[!UICONTROL Priority]|Enter a value for the pricing rule priority. A priority value equal to `1` is the highest priority. When you have multiple pricing rules, you can use the priority value to determine which rule is applied first. This field is required to use the **Discard Subsequent Rules** feature.|
|[!UICONTROL Discard Subsequent Rules]|Used to allow or prevent multiple pricing rules from stacking and providing additional discounts. To discard subsequent rules, a pricing rule must have a value defined for **[!UICONTROL Priority]**. Options:<ul><li>**[!UICONTROL Yes]** - Choose when you do not want any other pricing rules that may apply to a product to be applied. Discarding subsequent rules means that, when multiple pricing rules apply to the same product, only the pricing rule with the highest defined priority value is applied.</li><li>**[!UICONTROL No]** - Choose when you want to allow multiple pricing rules to apply to the same product. This option could result in stacking and multiple discounts applied to your listing price.</li></ul>|
