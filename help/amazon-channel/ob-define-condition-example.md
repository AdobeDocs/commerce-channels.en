---
title: 'Example: Define a Condition'
description: When creating your listing rules, define conditions for identifying the Commerce catalog products to be listed on the Amazon Marketplace.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
---
# Example: Define a Condition

## Conditions

Any areas in the conditions that are bold can be clicked to see the various options.

**Do not add conditions if all products within the selected website are eligible.**

>[!NOTE]
>
>There is a complex set of back-end processes to communicate with Amazon's systems directly. Based on the number of items you are attempting to list, and how busy Amazon's systems might be (such as Black Friday), it could take time for your items to be listed on Amazon.

See the Conditions section of [Creating a Cart Price Rule](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog-create.html).

## Define a condition

This process can be simple or detailed, depending on your catalog setup. You can set up your conditions so that when `ALL` or `ANY` of the define conditions are either `TRUE` or `FALSE` for a product, then the product is eligible to be listed on Amazon.

Conditions are based on existing product attribute values. To apply the rule to all products, leave the conditions section blank.

>[!NOTE]
>
>If you want to define a condition based on a specific product attribute, set the **[!UICONTROL Use for Promo Rule Conditions]** setting for the attribute to `Yes`. You can access this setting on the [Storefront Properties](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes-add.html) page for the attribute.

![Condition - line 1](assets/ob-listing-rule-conditions-start.png){width="500"}

The rule in this example defines a rule that sets Amazon eligibility for all catalog products that have the _Amazon FBA_ attribute set to `Yes`.

The rule statement has two bold links, which, when clicked, display the options for that part of the statement. If you save the condition without making changing a bold option, the rule applies to all your products.

- Click **[!UICONTROL ALL]** and chose either `ALL` or `ANY`.
- Click **[!UICONTROL TRUE]** and choose either `TRUE` or `FALSE`.
- To apply the rule to all products, leave the condition unchanged.

You can create different conditions by changing the combination of these values. For this example, the following condition is used:

`If ALL of these conditions are TRUE:`

1. Click the Add (![Add icon](assets/btn-add-grn.png)) icon at the beginning of the condition line and select an attribute on which to base the condition, such as a conditions combination or a product attribute.

   - **[!UICONTROL Conditions Combination]** - Choose to allow you to create another set of `All/Any` and `True/False` conditions inside the existing set.

      ![Conditions combination](assets/ob-conditions-combinations.png){width="500"}

   - **[!UICONTROL Product Attribute]** - The product attributes depend on the setup of the attribute. For an attribute to appear in the list, it must be configured for usage in promotional rule conditions. See the _Use for Promo Rule Conditions_ in [Product Attributes](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

      In the list under **[!UICONTROL Product Attribute]**, choose the attribute that you want to use as the basis of the condition. For this example, the selected condition is `Amazon FBA`.

      ![Condition line 2, part 2](assets/ob-condition-attribute-dropdown.png){width="350"}

      The selected condition appears in the statement, followed by two more bold links. The options differ depending on the product attribute you select.

      After you set the attribute, it cannot be changed. To change the attribute, you must delete the line and add the new attribute. You can delete a condition line by clicking the Delete (![Delete icon](assets/btn-del-red.png)) icon at the end of the line.

     1. Click **[!UICONTROL is]** and choose the comparison operator that describes the condition for products to meet.

         For this example, the comparison operator is `is`. The available options depend on the attribute selected in the previous step. Options could include different comparison options, such as matching values, not including or including at least one of a value, and greater than, equal to, and less than a numerical amount. In this example, the options are `is` and `is not`.

     1. Click **[!UICONTROL ...]** and choose the attribute value upon which the condition is based.

         The options depend on the attribute's setup. You may be prompted to select an option, or to enter text or numerical values for the condition. For this example, the selection is `Yes`.

         The selected item appears in the statement to complete the condition.

         ![Condition line 2, part 3](assets/ob-listing-rule-condition-is.png){width="500"}

   This condition is complete. As stated, this condition means that any product in your [!DNL Commerce] catalog that has the Amazon FBA attribute set to a value of `Yes` is eligible for listing to Amazon for the region and store. You can add more condition lines to further narrow your eligible products.

1, To add another condition line to the statement, return to step 1 and repeat the process until all desired conditions are complete.

You can delete a line of the condition statement at any time by clicking the Delete (![Delete icon](assets/btn-del-red.png)) icon at the end of the line.
