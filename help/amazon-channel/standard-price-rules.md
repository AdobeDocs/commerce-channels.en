---
title: Amazon sales channel - Standard price rule actions
description: Use standard price rule actions to increase or decrease an Amazon listing price relative to the Commerce catalog price (or price source).
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
---
# Standard price rule actions

A standard price rule action allows you to increase or decrease an Amazon listing price by a specific percentage or fixed dollar amount relative to the [!DNL Commerce] catalog price (or price source).

Sections of a standard price rule action include:

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## Configure price rule actions

1. For **[!UICONTROL Rule Type]**, choose `Standard price rule`.

   This option disables the other fields in the _[!UICONTROL Select Rule Type]_ section.

1. Expand the _[!UICONTROL Price Adjustment]_ section, if needed.

1. For **[!UICONTROL Price Action]**, choose an option to determine how you want change the *[!UICONTROL Magento Price Source]* (defined in your [Listing Price](./listing-price.md)) value.

   - `Decrease By` - Choose when you want the value to be decreased before listing to Amazon.

   - `Increase By` - Choose when you want the value to be increased before listing to Amazon.

1. For **[!UICONTROL Apply]**, choose an option an option to determine how you want the defined *[!UICONTROL Magento Price Source]* defined in your [Listing Price](./listing-price.md) value to be adjusted:

   - `Apply as percentage` - Choose when you want the defined *[!UICONTROL Magento Price Source]* defined in your [Listing Price](./listing-price.md) value adjusted by a percentage

   - `Apply as fixed amount` - Choose when you want the defined *[!UICONTROL Magento Price Source]* defined in your [Listing Price](./listing-price.md) value adjusted by a fixed amount.

1. For **[!UICONTROL Adjustment Amount]** (required), enter the numerical value for the price adjustment.

   - When *[!UICONTROL Apply]* is set to `Apply as percentage`, enter the percent value (example: enter `25` for a 25% percent price adjustment).

   - When *[!UICONTROL Apply]* is set to `Apply as fixed amount`, enter the numerical value for the fixed amount (example: enter `25` for a $25 fixed price adjustment).

1. When complete, click **[!UICONTROL Save pricing rule]**.

![Standard price rule](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

|Field|Description|
|---|---|
|[!UICONTROL Rule Type]|Select `Standard price rule`.|
|[!UICONTROL Price Action]|Options:<ul><li>**[!UICONTROL Decrease By]** - Choose when you want the defined [!DNL Commerce] price source value to be decreased before listing to Amazon.</li><li>**[!UICONTROL Increase By]** - Choose when you want the defined [!DNL Commerce] price source value to be increased before listing to Amazon.</li></ul>|
|[!UICONTROL Apply]|Options:<ul><li>**[!UICONTROL Apply as percentage]** - Choose when you want the defined [!DNL Commerce] price source value adjusted by a percentage.</li><li>**[!UICONTROL Apply as fixed amount]** - Choose when you want the defined [!DNL Commerce] price source value adjusted by a fixed amount.</li></ul>|
|[!UICONTROL Adjustment Amount]|Required.<br><br>If you choose `Apply as percentage` for *[!UICONTROL Apply]*, enter the percent value (example: enter `25` for a 25% percent adjustment).<br><br>If you chose `Apply as fixed amount` for *[!UICONTROL Apply]*, enter the numerical value for the fixed amount (example: enter `25` for a $25 fixed adjustment).|
