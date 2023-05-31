---
title: Amazon sales channel - Price rule examples
description: To help you design your pricing rules for Amazon listings, review these examples based on common scenarios.
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
---
# Price rule examples

## Standard price rule examples

### Discard subsequent rules

The ability to discard subsequent rules is a great feature inside pricing rules that prevents multiple pricing rules from stacking and providing unintended additional discounts. To discard subsequent rules, a pricing rule must use the priorities that are set in the _[!UICONTROL Priority]_ section of [Pricing Rule General Settings](./pricing-rule-general-settings.md).

If **[!UICONTROL Discard Subsequent Rules]** is set to `Yes`, the rules with lower priority (higher numbers) do not apply to the eligible products.

For example, let's say there are three pricing rules:

| Example|Rule Name | Priority | Discard Subsequent Rule |
|----------|----|----|----|
| 1| 10% off sale products | 1 | No |
| 2| $2 off sale products | 2 | Yes |
| 3| 5% off all products | 3 | No |

In this scenario, rule #1 and #2 apply to the eligible products. Rule #3 only applies to eligible products not contained within rule #2 because it has a lower priority than example #2 and **[!UICONTROL Discard Subsequent Rules]** is set to `Yes`. So, the eligible products in the sale category would receive a 10% discount and $2 off the Amazon listing price.

### Applying two standard price rules

| Field | Setting - Rule 1 | Setting - Rule 2 |
|----------|----|----|
| [!UICONTROL Rule Name] | Rule-1 | Rule-2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Standard price rule | Standard price rule |
| [!UICONTROL Price action] | Decrease By | Decrease By |
| [!UICONTROL Apply] | Apply as percentage | Apply as fixed amount |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Product 1

Price: $45.49

Rule 1 applied: $45.49 x (0.9) = $40.94

Rule 2 applied: $40.94 - $10.00 = $30.94

The final price after Rule 1 and Rule 2 are applied: $30.94

#### Product 2

Price: $47.76

Rule 1 applied: $47.76 x (0.9) = $42.98

Rule 2 applied: $42.98 - $10.00 = $32.98

The final price after rule 1 and rule 2 are applied: $32.98

## Intelligent repricing rule examples

### Buy Box price with Floor Price Source = Price

| Field | Setting |
|----------|----|
| [!UICONTROL Rule Name] | Rule-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligent repricing rule |
| [!UICONTROL Competitor Price Source] | Use "Buy Box" Price |
| [!UICONTROL Price Action] | Match Competitor Price |
| [!UICONTROL Floor Price Source] | Price |
| [!UICONTROL Floor Price Action] | Match |

#### Product 1

Price: $15

[Buy Box](./buy-box-competitor-pricing.md) price from Amazon: $10

Because the [Buy Box](./buy-box-competitor-pricing.md) price is less than the original price, the product is listed at the original price.

The final price after the rule is applied: $15

#### Product 2

Price: $5

[Buy Box](./buy-box-competitor-pricing.md) price from Amazon: $10

Because the [Buy Box](./buy-box-competitor-pricing.md) price is greater than the original price, the product is listed at the [Buy Box](./buy-box-competitor-pricing.md) price.

The final price after the rule is applied: $10

### Buy Box price with Floor Price Source = Price and a 20% price decrease

| Field | Setting |
|----------|----|
| [!UICONTROL Rule Name] | Rule-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligent repricing rule |
| [!UICONTROL Competitor Price Source] | Use "Buy Box" Price |
| [!UICONTROL Price Action] | Match Competitor Price |
| [!UICONTROL Floor Price Source] | Price |
| [!UICONTROL Floor Price Action] | Decrease By |
| [!UICONTROL Apply] | Apply as a percentage |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### Product 1

Price: $20

Calculated Floor Price: $16

[Buy Box](./buy-box-competitor-pricing.md) price from Amazon: $15

Because the [Buy Box](./buy-box-competitor-pricing.md) price is less than the Calculated [Floor Price](./floor-price.md), the product is listed at the Calculated [Floor Price](./floor-price.md).

The final price after the rule is applied: $16

#### Product 2

Price: $15

Calculated [Floor Price](./floor-price.md): $12

[Buy Box](./buy-box-competitor-pricing.md) price from Amazon: $15

Because the [Buy Box](./buy-box-competitor-pricing.md) price is greater than the Calculated [Floor Price](./floor-price.md), the product is listed at the [Buy Box](./buy-box-competitor-pricing.md) price.

The final price after the rule is applied: $15

#### Product 3

Price: $17

Calculated Floor Price: $13.60

[Buy Box](./buy-box-competitor-pricing.md) price from Amazon: $15

Because the [Buy Box](./buy-box-competitor-pricing.md) price is greater than the Calculated [Floor Price](./floor-price.md), the product is listed at the [Buy Box](./buy-box-competitor-pricing.md) price.

The final price after the rule is applied: $15

### Lowest Price with all competitor's prices and use all competitor's product conditions

| Field | Setting |
|----------|-----|
| [!UICONTROL Rule Name] | Rule-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligent repricing rule |
| [!UICONTROL Competitor Price Source] | Use Lowest Competitor Price |
| [!UICONTROL Minimum Positive Feedback] | All Competitor Prices |
| [!UICONTROL Conditional Variance] | Use all competitor's product conditions |
| [!UICONTROL Price Action] | Match Competitor Price |
| [!UICONTROL Floor Price Source] | Price |
| [!UICONTROL Floor Price Action] | Match |

| Price | Condition |
|----------|----|
| $17 | New |
| $15 | New |
| $14 | Used; Very Good |
| $13 | Used; Good |

#### Product 1

Price: $10

Condition: New

Because the lowest competitor price for the New condition is $15, the product is listed at $15.

The final price after the rule is applied: $15

#### Product 2

Price: $10

Condition: Used; Acceptable

Because the [lowest competitor price](./lowest-competitor-pricing.md) for the Used condition is $13, the product is listed at $13.

The final price after the rule is applied: $13

### Intelligent repricing rule combining ceiling price, currency conversion, and VAT

| Field | Setting |
|----------|-----|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $10 |
| [!UICONTROL Currency conversion] | 1.25Euro:1USD |

[Ceiling price](./optional-ceiling-price.md) in the European (VAT) market: $10 x 1.25 = $12.50

When the [ceiling price](./optional-ceiling-price.md) in the European (VAT) market is hit, the VAT is calculated and added.

Final price after VAT: $12.50 x (1.1) = $13.75

### Combining multiple pricing rules, ceiling price, currency conversion, and VAT

#### Intelligent pricing rule (from previous example)

| Field | Setting |
|----------|----|
| Priority | 1 |
| VAT | 10% |
| Ceiling price source | $10 |
| Currency conversion | 1.25Euro:1USD |

[Ceiling price](./optional-ceiling-price.md) in the European (VAT) market: $10 x 1.25 = $12.50

Final price after VAT: $12.50 x (1.1) = $13.75

#### Standard pricing rule

| Field | Setting |
|----------|-----|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Increase By |
| [!UICONTROL Apply] | Apply as fixed amount |
| [!UICONTROL Adjustment Amount] | $5.00 |

When the [ceiling price](./optional-ceiling-price.md) is hit, the standard pricing rule is applied on top of the intelligent pricing rule.

Final price after the standard pricing rule is applied: $13.75 + $5.00 = $18.75

### Price adjustment

In this example, the most competitive price is defined by looking at the Amazon [competitor's lowest price](./lowest-competitor-pricing.md) with a 95% positive feedback and a minimum feedback count of 1,000 merchant reviews.

![Price adjustment example](assets/amazon-price-adjustment-example.png){width="600" zoomable="yes"}

After running this search based on these parameters, the competitive price comes back at $25.

From here, there are three different [price rule action](./pricing-rule-actions.md) choices based on this lowest price.

|Field|Description|
|--- |--- |
|[!UICONTROL Price Action]|Options:<ul><li>**[!UICONTROL Decrease By]** – This option decreases your listing price relative to the [lowest competitor price](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** – This option increases your listing price relative to the [lowest competitor price](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** – This option changes your Amazon listing price to match the lowest price based on the parameters. In the example, the Amazon listing price is $25.</li></ul>|
|[!UICONTROL Apply]|Options: Apply as percentage / Apply as fixed amount|
|[!UICONTROL Adjustment Amount]|Numerical value to define the percentage or fixed amount for the discount to be applied. <br>These selections result in taking the lowest price and setting it at $0.01 less.|

### Floor price

| Field | Setting |
|----------|----|
| [!UICONTROL Floor Price Source] | Cost = $5 |
| [!UICONTROL Floor Price Action] | Increase By |
| [!UICONTROL Apply] | Apply as percentage |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[Floor price](./floor-price.md) calculation = Floor Price Source `$5` x Floor Adjustment Amount `5%` = $5.25

When the intelligent pricing rule is applied, it does allow the listing price to be lower than $5.25 for this specific product when the cost is $5.
