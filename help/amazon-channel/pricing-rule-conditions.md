---
title: Amazon sales channel - Price rule conditions
description: Use the price rule conditions to determine which products are eligible for the listing price rule.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
---
# Price rule conditions

Conditions determine which products are eligible for the price rule. Defining the conditions for your Amazon pricing rules follow the same logic and process as defining the conditions for [Cart Price Rules](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) in [!DNL Commerce].

>[!IMPORTANT]
>
>If your price rule applies to all products in your [!DNL Commerce] catalog, then leave this section blank.

Any areas in the conditions that are bold can be clicked to see the various options.

## Example: build a price rule condition

This process can be simple or detailed, depending on your catalog configuration. You can define your conditions so that when `ALL` or `ANY` of the conditions are either `TRUE` or `FALSE` for a product, then the product is eligible for the pricing rule to be applied.

Conditions are based on your [product attributes](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html). To apply the rule to all products, leave the conditions section blank.

>[!NOTE]
>
>If you want to define a condition based on a specific product attribute, **Use for Promo Rule Conditions** for the attribute must be set to `Yes` in your [Storefront Properties](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html) for the attribute.

![Price rule condition - line 1](assets/ob-price-rules-condition-1.png){width="600" zoomable="yes"}

This example defines a rule that applies a 25% discount to all products that are defined in the `Books` category.

The rule statement has two bold links, which, when clicked, show the options for that part of the condition statement. If you save the condition without changing a bold option, the rule applies to all your products.

- Click **[!UICONTROL ALL]** and choose either `ALL` or `ANY`.
- Click **[!UICONTROL TRUE]**, and choose either `TRUE` or `FALSE`.
- To apply the rule to all products, leave the condition unchanged.

You can create different conditions by changing the combination of these values. For this example, the following condition is used:

   `If ALL of these conditions are TRUE:`

1. To show available attributes for which the condition applies, click the Add (![Add icon](assets/btn-add-grn.png)) icon at the beginning of the condition line and select an attribute on which to base the condition.

   **[!UICONTROL Conditions Combination]** -  Choose to create another set of `All/Any` and `True/False` conditions inside the existing condition.

   ![Price rule conditions combination](assets/ob-conditions-combinations.png){width="500"}

   **[!UICONTROL Product Attribute]** - The available product attributes depend on the [setup of the attribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html). For an attribute to show in the list, *[!UICONTROL Use for Promo Rule Conditions]* for the attribute must be set to `Yes` in your storefront properties.

   - For **[!UICONTROL Product Attribute]**, choose the attribute that you want to define as the base of the condition. For this example, the selected condition is `Category`.

      ![Price rule condition - line 2, part 2](assets/ob-price-rule-condition-2.png){width="500"}

      The selected condition appears in the statement, followed by two more bold links. The options differ depending on the product attribute you select.

      After you set the attribute, it cannot be edited. To change the attribute, you must delete the line and add the new attribute. You can delete a condition line by clicking the Delete (![Delete icon](assets/btn-del-red.png) icon at the end of the line.

   - Click **[!UICONTROL is]** and choose the comparison operator that describes the condition for products to meet.

      For this example, the comparison operator is `is`. The available options depend on the attribute selected in the previous step and could include different comparison options. Options can include matching values, not including or including at least one of a value, and greater than, equal to, and less than a numerical amount. In this example, the options are `is` and `is not`.

   - Click **[!UICONTROL ...]** and choose the attribute value upon which the condition is based. The options depend on the attribute's setup.

      You might be prompted to select an option or enter a value for the condition. For this example, the field appears blank. To select your category(ies) for the rule, click the chooser icon (![Chooser icon](assets/btn-chooser.png)) to show your selection options. This rule is for _Books_, select the **[!UICONTROL Books]** checkbox. The category number populates. To accept your category selections, click the green check mark icon (![Check mark icon](assets/btn-check-mark-green.png)).

      ![Price rule condition - line 2, part 3](assets/ob-price-rule-condition-3.png){width="500"}

      The selected item appears in the statement to complete the condition.

      ![Price rule condition - line 2, part 4](assets/ob-price-rule-condition-4.png){width="500"}

      This example condition is complete. As stated, this condition means that any product in your [!DNL Commerce] catalog that has a defined category of Books (`4`) is eligible for this pricing rule. You can add more condition lines to further narrow your eligible products.

1. To add another condition line to the statement, return to Step 1 and repeat the process until all desired conditions are complete.

    You can delete a line of the condition statement at any time by clicking the Delete (![Delete icon](assets/btn-del-red.png)) icon at the end of the line.
