---
title: "[!UICONTROL Amazon Stores] view"
description: Go to the Amazon Stores view to quickly review basic statistics for each of your Amazon stores, and access management options.
feature: Sales Channels, Storefront
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
---
# [!UICONTROL Amazon Stores] view

When viewing the Amazon sales channel home page, the _Amazon Stores_ view opens by default.

![Amazon Stores view](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

The _[!UICONTROL Amazon Stores]_ view shows a "store card" for each of your Amazon stores along with some basic statistics and management options. Summary information shown in each card includes each store status, date created, last updated date, listings that need attention (example: Incomplete Listings) and the assigned [!DNL Commerce] website.

When viewing the _[!UICONTROL Amazon Store]_ view, each store card allows you to:

- To open a store [dashboard](./amazon-store-dashboard.md), click **[!UICONTROL View Store]**.

- To change a store status or delete a store, click **[!UICONTROL Action]** and choose:

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - Choose to change the status of the store to `Active` or `Inactive`, respectively.

      Changing an `Inactive` store to `Active` status activates listings and order activity for the store, using the stores current store settings (such as listing settings, price rules, and overrides).

      Changing a store status from `Active` to `Inactive` status suspends listings and order activity for the store. An Inactive store retains all store settings and listings, but temporarily stops the synchronization of pricing, quantity, and order management until the store is changed back to `Active` status. This feature allows you to control your store activity at the Regional level without the need to recreate or reintegrate your Amazon store or the loss of historical order and sales data.

   - **[!UICONTROL Delete]** - Choose to delete a store that is no longer needed.

      Choose when you wish to delete an existing Amazon store and its integration settings with your [!DNL Amazon Seller Central] account. Deleting the account removes the store from Amazon sales channel, along with all account settings, listings, logs, and other information related to this store. The store cannot be retrieved after deletion, a new store must be created.

>[!NOTE]
>To change the website assigned to the store during integration, you must delete the store and add the store again with the different website defined during store integration.

| Store Card     | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Top section    | Includes: <br>The region icon for the store, defined during [store integration](./store-integration.md).<br> The assigned _[!UICONTROL Magento Website]_, defined during store integration.<br>The _[!UICONTROL Status]_ of your store. Options: **[!UICONTROL Active]** - Store integration is complete and verified with Amazon and is available for sales activity. **[!UICONTROL Inactive]** - Store integration is complete, but is not in use or available for sales activity. When `Inactive`, your Amazon sales are paused. When `Active`, sales revenue and additional settings save to update before activating.<br>The *[!UICONTROL Last Updated]* date of the most recent change to the Amazon store setup.<br>The *[!UICONTROL Created]* date when the Amazon store was created in Amazon sales channel. |
| Middle section | Includes a store activity summary chart for the last 30 days and includes and alert for any listings that need attention.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Bottom section | Includes the View Store and Action options.<br>To open the store [dashboard](./amazon-store-dashboard.md), click **[!UICONTROL View Store]**.<br>To activate, deactivate, or delete a store, click **[!UICONTROL Actions]**.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
