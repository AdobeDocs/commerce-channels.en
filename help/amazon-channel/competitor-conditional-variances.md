---
title: 'Intelligent Repricing Rule: Competitor Conditional Variances'
description: Determine your Amazon listing price based on competitor pricing and condition of the product by creating an intelligent repricing rule.
feature: Sales Channels, Configuration
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
---
# Intelligent Repricing Rule: Competitor Conditional Variances

Sections of an intelligent repricing rule include:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

An intelligent repricing rule uses Amazon competitors' pricing to determine your listing price. Competitors are other sellers that are listing the same products you are listing on Amazon.

If a product exists with the same condition, the base match price is the [lowest competitor](./lowest-competitor-pricing.md) price with the same condition. If no competitor product matches your condition, the base match price then goes through other available competitor conditions starting with New, Refurbished, and continuing down through available conditions. After a condition is found, the base match price will be the lowest price within that condition.

If you have a product listed with the condition `Used; Good` and the base match price, and a competitor has the same product in the same condition at a lower price, the competitor price is used. If a competitor does not exist with the same condition, the system checks for a competitor with the next condition, which is `New`. If a competitor is found with that condition, the lowest price is used.

## Configure competitor conditional variances

Define your condition variances in the _[!UICONTROL Competitor Conditional Variances]_ section.

For **[!UICONTROL Conditional Variance]**, choose an option:

- `Use all competitor's product conditions` - (Default) Choose when you want your product to compare against any available condition (if a match does not exist for the condition you are listing).

- `Use Only Matching Competitor's Product Condition` - Choose when you want your product to compare only against competitor's products in the same condition. If no match exists, the product is priced at the _Magento Price Source_ defined in your [Listing Price](./listing-price.md).

- `Apply Variance (if competitor's product condition differs)` - Choose to first try to compare against your matched product condition. If no matching condition exists, a variance (as a percentage) is applied relative to your product condition and the lowest competitor's condition.

   When the _[!UICONTROL Apply Variance]_ feature is chosen, additional variance fields display for each of your Amazon conditions. This feature allows you to use intelligent repricing rules when you offer products that are in a different condition than your competitors. To understand the calculation behind conditional variance, you must first understand that all variance is determined from a base match price.

   Conditional variance options that appear are based on your listing settings for `Condition` that are mapped to condition values using a [!DNL Commerce] [product attribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). For all mapped conditions, you can define a variance percentage of 1-100. The exception is collectibles, in which case a percentage greater than 100 may be applied.

![Intelligent repricing rule - competitor conditional variances](assets/amazon-competitor-cond-variances.png){width="500" zoomable="yes"}

| Field                                         | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Competitor Conditional Variances] | Options: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - If a match does not exist for the condition you are listing your product with, this option matches against any available condition. It first attempts to match your condition, and then works its way from the `New` condition to `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - This option matches against your product's condition. If no match exists, the product prices at the _[!UICONTROL Magento Price Source]_.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - This option first tries to match against your product condition. If no matching condition exists, it applies a variance (as a percentage) relative to your product condition and the lowest competitor's condition.</li></ul><br><br>The conditional variance options that appear based on your listing settings for Condition that are mapped to condition values using a [!DNL Commerce] [product attribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). For all mapped conditions, you can denote a variance percentage of 1-100. The exception is collectibles, in which case a percentage greater than 100 may be applied.<br><br>This feature allows you to use intelligent repricing rules when you offer products that are in a different condition than your competitors. To understand the calculation behind conditional variance, you must first understand that all variance is determined from a base match price. |

## Calculate the conditional variance base

- Base Match Condition Variance (BMC) = The variance for the condition of your base match price competitor. Using the earlier example, BMC is the variance for the `New` condition.
- Merchant Condition Variance (MCV) = The variance for the condition of your product. Using the earlier example, MCV = the variance for the `Used; Good` condition.
- Base Match Price (BMP) = $7.99 (explained above)

The formula for calculating conditional variance base is as follows:

![conditional variance base calculation formula](assets/amazon-cond-variance-calc-1.png){width="300"}

## Example

The conditional variance settings are as follows:

![example conditional variance settings](assets/amazon-cond-variances.png){width="500" zoomable="yes"}

- BMC = 100 (Competitor condition = New)
- MCV = 80 (Merchant condition = Used; Good)
- BMP = $7.99 (Base match price = The lowest price of the matched competitor condition)

![conditional variance base calculation example](assets/amazon-cond-variance-calc-2.png){width="300"}

Using the conditional variance base calculation from above, your conditional variance base = $6.39. This calculation is the competitor price source used for your price rule actions, explained further in [Price Adjustment](./price-adjustment.md).
