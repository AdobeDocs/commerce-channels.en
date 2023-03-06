---
title: Amazon Order Details
description: View details for your Amazon Marketplace orders in the Adobe Commerce or Magento Open Source Admin.
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
---
# Amazon Order Details

![Amazon order details](assets/amazon-order-details-header.png)

## View Amazon order details

1. Click **[!UICONTROL View Store]** on the store card.

1. In the _[!UICONTROL Recent Orders]_ section, click an order number.

    The _[!UICONTROL Amazon Order Details]_ page opens.

>[!NOTE]
>
>If you have order import enabled in your [Order Settings](./order-settings.md) and the order is [fulfilled by Amazon (FBA)](./fulfilled-by.md), you may see dummy data for some fields in the order details. Amazon does not send the following data for FBA orders.
>
> - `AddressType`
> - `AddressLine1`
> - `AddressLine2`
> - `AddressLine3`
> - `BuyerName`
> - `Phone`
> - `PurchaseOrderNumber`
> - `RecipientName`
> - `CustomizedURL`
> - `GiftMessageText`

### Order and Shipping Details tab

The _[!UICONTROL Order and Shipping Details]_ tab shows detailed order information, as received from Amazon.

>[!IMPORTANT]
>
>Amazon accepts non-standard address information that cannot be imported into Amazon sales channel, thus preventing the state/country codes from updating correctly for some orders. To correct address errors, the following fields are editable in the order details:
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>Do not forget to click **Save Order** after making edits.

![Order and Shipping Details](assets/amazon-order-details.png)

### Order Items tab

The _[!UICONTROL Order Items]_ tab shows all items associated with the Amazon order, as received from Amazon.

![Order Item Details](assets/amazon-order-item-details.png)

### Tracking tab

The _[!UICONTROL Tracking]_ tab shows tracking information associated with the Amazon order.

![Tracking details](assets/amazon-order-tracking-details.png)
