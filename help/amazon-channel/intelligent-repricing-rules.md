---
title: 'Intelligent Repricing Rule: Select Rule Type'
description: Determine your Amazon listing price according to competitor pricing by creating an intelligent repricing rule.
exl-id: 2690323a-a076-484b-a437-adadb08094f5
---
# Intelligent Repricing Rule: Select Rule Type

>[!IMPORTANT]
>
>Intelligent repricing rules do not function properly if the Amazon region is set to `Inactive` status, as it is during onboarding. Your pricing calculations depend on your shipping rates, and your region must be in `Active` status for your shipping rates to sync from Amazon.<br><br>
>
>To update your region status in your Amazon account, go to Settings > Account Info > Vacation Settings. Refer to [Amazon: Listing Status for Vacations](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/"target="_blank)

An intelligent repricing rule uses Amazon competitors' pricing to determine your listing price. Competitors are other sellers who list the same products as yours on Amazon.

Sections of an intelligent repricing rule include:

- Select Rule Type
- [Competitor Conditional Variances](./competitor-conditional-variances.md)
- [Price Adjustment](./price-adjustment.md)
- [Floor Price](./floor-price.md)
- [Optional Ceiling Price](./optional-ceiling-price.md)

## Configure the rule type

Define the rule type in the _[!UICONTROL Select Rule Type]_ section.

1. For **[!UICONTROL Rule Type]**, choose `Intelligent repricing rule`.

   This setting enables the _[!UICONTROL Competitor Price Source]_ field and the [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md), and [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) sections.

1. For **[!UICONTROL Competitor Price Source]**, choose an option:

   - **[!UICONTROL Use "Buy Box" Price]** - Choose when you want to adjust your Amazon pricing based on the Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) seller price. A [!DNL Buy Box] price exists when multiple sellers on Amazon offer the same product. Amazon defines the [!DNL Buy Box] seller based on performance requirements. Merchants seek to win the [!DNL Buy Box] seller status and offer maximum visibility of their product listings.

   - **[!UICONTROL Use Lowest Competitor Price]** - Choose when you want to compare and adjust your listing price to competitor pricing for the same product. When chosen, the _[!UICONTROL Minimum Positive Feedback]_ and _[!UICONTROL Minimum Feedback Count]_ fields are enabled.

1. If enabled, choose an option for **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - Choose when you want to compare and adjust your pricing based on all competitor prices for the same product.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Choose when you want to limit the competitors to whom the price is compared for the same product. This setting narrows the competitors further by requiring their listing to have a minimum of the chosen percentage of positive feedback before applying the lowest price rule.

1. If enabled, enter a numerical value for **[!UICONTROL Minimum Feedback Count]**.

   This optional numerical value further narrows down the competitive pricing. For example, if a merchant has a 95% positive feedback rating, but only has a feedback count of `20`, it might not be a competitor you want to modify your pricing against. However, if you enter a value of `1000`, it would require that the merchant has 95% positive feedback and a minimum of 1000 merchant reviews.

>[!NOTE]
>
>You might use these competitor pricing and feedback options to avoid basing your pricing against a competitor who has poor feedback and is selling a lower quality product.

![Intelligent repricing rule - select rule type](assets/ob-intelligent-price-rule-type.png){width="600" zoomable="yes"}

|Field|Description|
|--- |--- |
|[!UICONTROL Rule Type]|Select a rule type. Options:<ul><li>**[!UICONTROL Standard price rule]** - This rule type allows you to increase or decrease the Amazon listing price by a specific percentage or fixed dollar amount relative to the _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - This rule type allows you to adjust your Amazon listing price, based on competitor's pricing. When chosen, the _[!UICONTROL Minimum Positive Feedback]_ and _[!UICONTROL Minimum Feedback Count]_ fields are enabled.</li></ul>|
|[!UICONTROL Competitor Price Source]|Select the desired price source. Options:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Choose this option when you want to adjust your Amazon pricing based on the Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) seller price. A [!DNL Buy Box] price exists when multiple sellers on Amazon offer the same product. Amazon defines the [!DNL Buy Box] seller based on performance requirements. Merchants seek to win the [!DNL Buy Box] seller status and offer maximum visibility of their product listings.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - Choose this option when you want to compare and adjust your listing price to the [lowest competitor pricing](./lowest-competitor-pricing.md) for the same product. When chosen, the _[!UICONTROL Minimum Positive Feedback]_ and _[!UICONTROL Minimum Feedback Count]_ fields are enabled.</li></ul> |
|[!UICONTROL Minimum Positive Feedback]|Only active if `Use Lowest Competitor Price` is chosen. Options:<ul><li>**[!UICONTROL All Competitor's Prices]** - Choose when you want to compare and adjust your pricing based on all competitor prices for the same product.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - Choose when you want to limit the competitors to whom you compare and adjust your pricing. This setting narrows your competitors further by requiring their listing to have a minimum of the chosen percentage of positive feedback and then use the lowest price of that subset of competitors.</li></ul> |
|[!UICONTROL Minimum Feedback Count]|Only active if `Use Lowest Competitor Price` is chosen. This optional numerical value further narrows the competitive pricing comparison. For example, if a merchant has a 95% positive feedback rating but only has a feedback count of `20`, it might not be a competitor you want to modify your pricing against. However, if you enter a value of `1000`, it would require that the merchant has 95% positive feedback and a minimum of 1000 merchant reviews. |
