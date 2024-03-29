---
title: Return and Refund Orders
description: Instructions for issuing full or partial refunds for return requests received from [!DNL Walmart Marketplace] from [!DNL Channel Manager] for Adobe Commerce and Magento Open Source.
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
---
# Return and Refund Orders

When a buyer requests a return for order items purchased through [!DNL Walmart Marketplace], Walmart creates a return request. [!DNL Channel Manager] monitors the marketplace channel for these requests and automatically synchronizes the return request information to Channel Manager.

On the Commerce side, the return request initiates the following workflow:

1. Channel Manager creates a corresponding return request with a received status and adds the return ID number ([!UICONTROL RMA #]) to the [!UICONTROL Returns] dashboard. On the [!DNL Orders] dashboard, the status detail for the order associated with the return updates to include a [!UICONTROL Return requested] link to view and process the return.

1. Merchants process the refund associated with the return by creating a Credit Memo following the [Adobe Commerce refund workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html). All refunds are processed using the offline method. 

1. [!DNL Channel Manager] sends a refund update to Walmart marketplace so the return status can be updated to reflect the completed refund from Adobe Commerce.

In the storefront Admin, you can view and process returns from Channel Manager by opening the sales channel store and selecting **[!UICONTROL Returns]**.

![Channel Manager Returns dashboard to process refunds for return requests received from [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>You can only process refunds for shipped orders. In [!DNL Channel Manager], the order status must be [!UICONTROL Shipped]. In [!DNL Walmart Marketplace] Seller account, the order must be [!UICONTROL Delivered].

## Returns Controls and Column Descriptions

The following tables describe the controls and columns available for [!DNL Channel Manager] returns.

**Controls for [!UICONTROL Returns]**

<table>
<tr>
<td><strong>Control</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>Filter the view by selecting one of the [!UICONTROL Return Status] cards.</td>
</tr>
<tr>
<td>Status Details</td>
<td>For return entries with the [!UICONTROL Received] or [!UICONTROL Refunded] status, you can create or view the credit memo for the refund by selecting the linked text in the Status Details column.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>To view order details, select the [!DNL Commerce] order number in the [!UICONTROL Order] table to open the Commerce order.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>To modify the channel configuration, select channel Walmart Connection credentials, mapped attributes, or shipping identifiers, settings  select the [!DNL Commerce] order number in the [!UICONTROL Order] table. Then, use [!DNL Commerce] order options to process the order.</td>
</tr>
</table>

**Column descriptions**

<table>
<tr>
<td><strong>Field</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>The Return Merchandise Authorization number associated with the return request received from [!DNL Walmart Marketplace]. This number is generated by Walmart Marketplace [!UICONTROL Returns] when the return process is initiated.</td>
</tr>
<tr>
<td>[!DNL Commerce] Order #</td>
<td>The [!DNL Commerce] order number associated with the items included in the return request from Walmart Marketplace. View order details by selecting the order number.</td>
</tr>
<tr>
<td>Requested</td>
<td>The date the return was requested on the [!DNL Walmart Marketplace]
converted to local time.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>The date that the return must be refunded by to meet [!DNL Walmart Marketplace] [requirements](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&article=000007176f) converted to local time.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>Lists the SKU and quantity for each item listed in the return.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>The total value to be refunded for the returned items.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>Indicates the current return status in the [!DNL Commerce] return workflow–<i>Received</i>, <i>Refunded</i>, or <i>Error</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>For received and refunded return entries, status details provide a link to access the credit memo for refund processing. If an error occurs during the [!DNL Channel Manager] synchronization process between Adobe Commerce and [!DNL Walmart marketplace], this field provides the error description.</td>
</tr>
</table>

## Return Status

[!UICONTROL Return Status] provides information about the current state of [!DNL Walmart Marketplace] return requests managed from Adobe Commerce or Magento Open Source.

Return status updates occur when [!DNL Channel Manager] receives an return request from the [!DNL Walmart Marketplace] or when the [!DNL Commerce] credit memo is created to process the refund for the returned items.

Returns can have the following statuses:

* **[!UICONTROL Received]**–This is the initial status of the return request received from the [!DNL Walmart Marketplace] store. The merchant can process the refund for the return by selecting **[!UICONTROL Create credit memo]** in the [!UICONTROL Status details].

* **[!UICONTROL Refunded]**—Indicates that a credit memo has been created to issue a refund for the returned items. Merchants can view refund information by selecting **[!UICONTROL View credit memo]** in the [!UICONTROL Status details].

* **[!UICONTROL Error]**—Return requests that have errors. Errors can occur when the return request from Walmart has missing or incorrect data. Or, if [!DNL Channel Manager] cannot send the refund update notification to Walmart.

## Return scenarios

The following scenarios describe how to issue refunds for different types of return requests from [!DNL Channel Manager].

* **Full return**—If the Walmart Marketplace return request is for all items in the order, update the credit memo quantity to refund all items.

* **Partial return**–If the Walmart Marketplace return request is for only some order items, update the credit memo quantity only for the items to be refunded.

* **Return already refunded through Walmart Marketplace**–In some cases, a refund is processed on [!DNL Walmart Marketplace] before you process the return in Channel Manager. For example, if a Commerce order is not refunded within the 48-hour refund processing window required by Walmart, Walmart automatically refunds the order. When this happens, Channel Manager still synchronizes the return request to Adobe Commerce so you can process the return and issue the credit memo. This workflow ensures that the order detail in [!DNL Commerce] matches the order information in Walmart Marketplace.

>[!NOTE]
>
> It can take up to five minutes for refund updates to synchronize to [!DNL Walmart Marketplace]. You can check the current return status from the [!DNL Channel Manager] [!UICONTROL Returns] dashboard.

## Process a refund request

1. Open the [!UICONTROL Returns] dashboard for your sales channel store.

   * From the Admin, select **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Open the store view by selecting the eye icon for a sales channel store.

   * You can review the returns by selecting the **[!UICONTROL Returns]** tab.

     You can also access return information from the [!UICONTROL Orders] page. Look for [!UICONTROL Shipped] orders that have a return request. Then, select the `Return requested` link in the [!UICONTROL Status Details] column to view and process the request.

1. From the Returns table, find a return with the *[!UICONTROL Received]* status.

1. From the items column, review the list of order items and quantity to refund.

1. Process the refund by issuing a credit memo.

   * From the [!UICONTROL Status Details] column, select **[!UICONTROL Create credit memo]** to open the Order detail page in [!DNL Commerce].

     If the order has not been invoiced, the Order detail page displays an error message prompting you to create one. Select **[!UICONTROL Create invoice]**. Then, [create and save the invoice](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html).

   * On the Order detail page, select **[!UICONTROL Credit Memo]**.

   * In [!UICONTROL Items to Refund] section of the [!UICONTROL Credit Memo], update the **[!UICONTROL Qty to refund]** and **[!UICONTROL Return to Stock]** information for the items included in the return request.

     Make sure that return only the items listed in the return request.

   * To add a comment, enter the text in the **[!UICONTROL Credit Memo Comments]**

   * Select **[!UICONTROL Refund Offline]**.

After completing the refund, [!DNL Channel Manager] updates the return status in the [!UICONTROL Returns] dashboard to [!UICONTROL Refunded] and synchronizes the update to Walmart to update the return status in marketplace.


## View refund information for a return

You can view information about return requests and refund processing from the [!UICONTROL Returns] dashboard.

1. Open the Returns dashboard for your sales channel store.

   * From the Admin, select **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * Open the store view by selecting the eye icon for a sales channel store.

   * Select **[!UICONTROL Returns]**.

1. View refunded orders by selecting the **[!UICONTROL Refunded]** status card.

1. View refund details for a return by selecting **[!UICONTROL View credit memo]**.

   ![Credit memo to refund returned items for a [!DNL Walmart Marketplace] order](assets/refund-credit-memo-for-marketplace-order.png){width="600" zoomable="yes"}

>[!NOTE]
>
>After an order has been refunded, the [!UICONTROL Orders] dashboard does not show return information. To view return information, use the [!DNL Channel Manager] Returns dashboard. More detailed return and refund information is also available from the Order detail page.

## Fix return errors

Errors can occur when the return information is received from [!DNL Walmart Marketplace], or when [!DNL Channel Manager] synchronizes status updates from [!DNL Commerce] to [!DNL Walmart Marketplace].

If the synchronization operation for a return update fails, the [!DNL Channel Manager] Returns dashboard shows an *[!UICONTROL Error]* status for the return entry. To ensure that return and refund information is accurately reflected in Walmart Marketplace account, manually update the order in your [!DNL Walmart Marketplace] store.
